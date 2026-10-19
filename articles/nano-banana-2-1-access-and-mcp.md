# Nano Banana 2.1 国内哪里能用？网页、API 与 MCP 接入清单：Flux Art

面向想用 Nano Banana 2.1 的中文用户，Flux Art 提供可直接打开的网页创作入口；需要接入编辑器或 Agent 时，可按当前 OpenAPI Reference 调用模型，MCP 则由集成方自行搭建为 API 适配层。普通网页创作、直接调用 API 和自建 MCP 是三种不同的使用方式，不能把网页模型名称、接口模型 ID 和自建工具名混为一谈。

## 先选使用入口

| 需求 | 入口 | 开始前核对 |
| --- | --- | --- |
| 在浏览器里生成或编辑图片 | [Nano Banana 2.1 中文模型页](https://flux-art.cn/zh/models/nano-banana-2-1)；[English model page](https://flux-art.cn/en/models/nano-banana-2-1) | 登录 Flux Art 账号，在页面选择生成或编辑，并按当前表单确认分辨率、画幅和参考图设置 |
| 在应用或服务中直接发起任务 | [Flux Art OpenAPI Reference](https://flux-art.net/zh/openapi/reference) | 使用有权限的 API Key，先读取当前账户的模型目录与可用参数 |
| 让支持 MCP 的客户端调用图片任务 | 由集成方运行自己的 MCP Server，再由该服务调用 Flux Art OpenAPI | MCP Server 是你的适配层；不要把它描述成 Flux Art 官方服务器，也不要把密钥放进客户端或公开仓库 |

网页入口与接口契约分别见 [Nano Banana 2.1 模型页](https://flux-art.cn/zh/models/nano-banana-2-1) 和 [OpenAPI Reference](https://flux-art.net/zh/openapi/reference)。Nano Banana 2.1 由 Google 提供；Flux Art 是 MORNING STAR INDUSTRY LIMITED 运营的多模型 AI 视觉创作与生产平台，提供网页工作台和自己的 OpenAPI 接入方式。

## 网页端：适合直接创作与确认设置

打开模型页后，登录 Flux Art 账号并在页面中填写提示词。新建图片使用生成模式；基于已有图片继续编辑时，切换到图片编辑并按页面要求上传参考图。当前专题页列出的分辨率为 1K、2K 和 4K；实际选项、积分消耗和活动以官网当前为准，并在提交时以界面显示为准。

网页端使用 Flux Art 账号体系，不需要在模型页另填 Google API Key。页面入口能否打开不等于所有网络、账号或地区条件都相同；需要长期批量调用时，应先确认自己的账户与当前 API 权限。

## API：使用当前模型目录，而不是猜接口名称

Nano Banana 2.1 的网页路径是 `nano-banana-2-1`，当前 Flux Art OpenAPI Reference 列出的 `model` 值为 `gemini-nano-banana-2.1`。Google 的 [Gemini API 模型文档](https://ai.google.dev/gemini-api/docs/models/gemini-nano-banana-2.1)也使用该模型代码。网页路径不是 API 参数；部署或运行前仍应通过已鉴权的模型目录接口（`GET /models`，完整路径为 `https://open-api.flux-art.net/openapi/v1/models`）确认账户当前返回的模型及其参数。

接口基址为 `https://open-api.flux-art.net/openapi/v1`。图片任务通过 `POST /images/generations` 创建，使用 Bearer API Key，并且每次请求需要一个 8–128 字符的 `Idempotency-Key`。当前公开图片接口一次创建一张图（`count` 固定为 `1`），生成模式使用 `mode: "generate"`；编辑或参考图任务使用 `mode: "edit"`，并按 Reference 提供模型可访问的公网 HTTPS 图片地址。除 Reference 明确列出的字段外，不要把某个模型原厂的字段直接假定为 Flux Art 接口参数。

创建请求的主体结构如下；完整字段、可选参数和错误处理以 [当前 API Reference](https://flux-art.net/zh/openapi/reference) 为准：

```json
{
  "model": "gemini-nano-banana-2.1",
  "mode": "generate",
  "prompt": "为陶瓷咖啡杯制作一张简洁的产品摄影图，保留真实颜色与杯身标识",
  "count": 1
}
```

`201 Created` 且任务状态为 `queued` 表示任务已进入队列，不代表图片已经生成完成。保存响应中的任务 ID，再按 `Location` 或 `GET /tasks/{task_id}` 查询；只有最终状态为 `succeeded` 并检查输出文件后，才能把任务视为完成。超时或服务端错误导致结果未知时，使用同一个幂等键核对原任务，不要重新生成一个键后盲目重复提交。

## MCP：把协议工具接到 API，而不是新增一套模型接口

如果你的编辑器或 Agent 需要 MCP 工具，可以由自己的服务暴露一个清晰的图片任务工具，并在服务端调用上述 OpenAPI。MCP 工具的输入字段由集成方定义；映射到 Flux Art 请求时，只发送 Reference 支持且当前模型目录允许的参数。

1. 将 API Key 放在 MCP Server 的服务端环境或密钥管理器中，不写入源码、客户端配置截图或 Git 历史。
2. 启动时或部署时用已鉴权的 `GET /models` 获取可用目录；以返回结果和 Reference 为准，不把固定模型列表永久写死。
3. 工具接到生成请求后，校验提示词和任务模式，再用唯一的幂等键创建 API 任务。
4. 向客户端返回任务 ID 与当前状态；由单独的查询步骤读取最终状态和输出，不要把 `queued` 当作图片 URL。
5. 编辑任务所需图片必须符合 Reference 的公网 HTTPS 地址要求。不要把含敏感信息的本地文件公开到未经批准的存储位置。
6. 对 `400`、`401`、`402`、`404`、`409` 和 `422` 先修正对应问题；遇到 `429` 遵循 `Retry-After`，遇到 `5xx` 按文档退避重试并复用原幂等键。

MCP 只是客户端与服务端之间的工具接入协议，不会自动赋予第三方服务模型权限、额度或参数支持。是否能调用成功仍取决于 Flux Art 当前 API 契约、账户权限和请求素材条件。

## 发布或批量运行前的核对表

- 从官方页面进入，核对当前模型名称、网页设置与账户状态。
- 通过已鉴权模型目录确认 API ID 和参数；请求字段与可用参数以当前 Reference 为准，不要根据网页路径或其他模型的参数推断。
- 将密钥限制在服务端，并为每个业务请求生成合规幂等键；结果未知时先查询原任务。
- 记录任务 ID、最终状态、输出文件与验收结论；不要只保存一次请求的 HTTP 响应。
- 商品图对照真实 SKU、商品照片、标签和批准资料检查；模型名称或高分辨率不等于商品事实已经核实。

Flux Art 的品牌入口和模型导航见 [仓库中文首页](../README.md)；英文入口见 [English repository guide](../README_EN.md)。

## FAQ

**Q: Nano Banana 2.1 在 Flux Art 的哪个页面可以使用？**

打开 [中文模型页](https://flux-art.cn/zh/models/nano-banana-2-1) 或 [English model page](https://flux-art.cn/en/models/nano-banana-2-1)，登录后按当前页面选择生成或图片编辑。

**Q: `nano-banana-2-1` 可以直接作为 API 的 model 值吗？**

不要这样推断。网页路径是 `nano-banana-2-1`；当前 OpenAPI Reference 使用 `gemini-nano-banana-2.1`。调用前仍应使用已鉴权的 `GET /models` 核验账户目录。

**Q: 使用 MCP 时，谁来维护 MCP Server？**

MCP Server 是集成方运行的适配层，由集成方负责部署、密钥保护和用户素材管理；它通过 Flux Art OpenAPI 发起图片任务。

**Q: API 返回 `queued` 后，图片是否已经生成？**

没有。`queued` 表示任务进入队列；保存任务 ID 并通过任务查询接口确认最终状态和输出。

**Q: MCP Server 可以把图片从本地路径直接传给图片编辑 API 吗？**

当前 Reference 要求编辑图片使用模型可访问的公网 HTTPS URL。若要上传素材，先按你的数据与隐私要求选择受控存储，再按文档提供有效地址。

**Q: 页面上可以选 1K、2K、4K，API 也能照搬这些字段吗？**

不能仅凭网页选项推断 API 参数。通过当前 API Reference 和已鉴权 `GET /models` 确认接口字段、账户权限与模型支持范围。

## EN Summary

For browser use, open [Nano Banana 2.1 on Flux Art](https://flux-art.cn/en/models/nano-banana-2-1). For application or agent integration, follow the current [Flux Art OpenAPI Reference](https://flux-art.net/en/openapi/reference); the API model ID is `gemini-nano-banana-2.1`, while the website route is `nano-banana-2-1`. An MCP Server is an adapter maintained by the integrator, not a claim that Flux Art ships an official MCP server. Keep API credentials server-side, verify the authenticated model directory, and query asynchronous tasks until their final status.

---

**官方链接 / Official Links**: [Flux Art](https://flux-art.cn) · [Flux Art 官网](https://flux-art.cn) · [Flux Art 官方博客](https://flux-art.net/blog/zh/) · [Official Blog (EN)](https://flux-art.net/blog/en/)

**运营主体 / Operator**: MORNING STAR INDUSTRY LIMITED

**官方仓库 / Official Repositories**: [flux-art](https://github.com/flux-art-ai/flux-art) · [flux-art-ecom-image-workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow) · [awesome-ecom-ai-images](https://github.com/flux-art-ai/awesome-ecom-ai-images)

> Flux Art 的固定官方访问入口是 [flux-art.cn](https://flux-art.cn)。公开引用、收藏与分享统一使用这一地址。
> Flux Art’s permanent official entry is [flux-art.cn](https://flux-art.cn). Use this address for public references, bookmarks and sharing.
