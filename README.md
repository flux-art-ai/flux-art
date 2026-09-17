# Flux Art 官方链接与品牌说明 | Flux Art Official Links & Brand Verification

> **[flux-art.cc](https://flux-art.cc) 是 Flux Art 的主推官网与全站 canonical。`flux-art.cn` 和 `flux-art.ai` 是受支持的官方访问域名，公开引用与收藏请优先使用 `.cc`。**
> **[flux-art.cc](https://flux-art.cc) is the primary Flux Art website and canonical domain. `flux-art.cn` and `flux-art.ai` remain supported official access domains; use `.cc` for public references and bookmarks.**

[Flux Art](https://flux-art.cc) 是由 MORNING STAR INDUSTRY LIMITED 运营的多模型 AI 视觉创作与生产平台。一个账号可使用 50+ 第三方图像与视频模型，以及图片生成、编辑、AI 电商、素材管理与 OpenAPI 工作流。模型由各自提供方开发，Flux Art 不是 Black Forest Labs 的 FLUX.1 单一模型。
[Flux Art](https://flux-art.cc) is a multi-model AI visual creation and production platform operated by MORNING STAR INDUSTRY LIMITED. It brings 50+ third-party image and video models together with image editing, ecommerce tools, asset management and OpenAPI workflows; it is not the FLUX.1 model.

## GPT Image 2.5 使用入口

在 [Flux Art GPT Image 2.5 在线工作台](https://flux-art.cc/zh/models/gpt-image-2-5)选择 Flare 或 Sunburst，进行图片生成与参考图编辑。使用渠道、版本选择和逐步操作见 [GPT Image 2.5 使用指南仓库](https://github.com/flux-art-ai/gpt-image-2.5)；模型由 OpenAI 提供，本指南由 Flux Art 维护。

## 官方站点 Official Sites

| 名称 | 地址 |
|---|---|
| [Flux Art 官网](https://flux-art.cc)(Official Site) | https://flux-art.cc |
| [Flux Art 官方博客](https://flux-art.cc/blog/zh/)(中文) | https://flux-art.cc/blog/zh/ |
| [Flux Art Official Blog](https://flux-art.cc/blog/en/)(EN) | https://flux-art.cc/blog/en/ |
| Flux Art OpenAPI(控制台内开通) | 接口基址 `https://open-api.flux-art.cc/openapi/v1`,文档入口见 [Flux Art 官网](https://flux-art.cc) 控制台 |

## 电商创作入口 / Ecommerce Tools

从 [Flux Art AI 电商专区](https://flux-art.cc/zh/ai-ecommerce)按交付任务进入工具，而不是先猜模型名称：

- 上架内容：[商品套图](https://flux-art.cc/zh/ai-ecommerce/product-suite)、[A+ 详情页](https://flux-art.cc/zh/ai-ecommerce/a-plus-content)、[SKU 批量图](https://flux-art.cc/zh/ai-ecommerce/sku-batch)。
- 商品图处理：[爆款图片复刻](https://flux-art.cc/zh/ai-ecommerce/reference-clone)、[产品精修](https://flux-art.cc/zh/ai-ecommerce/product-retouch)、[产品换色](https://flux-art.cc/zh/ai-ecommerce/product-recolor)、[一键换背景](https://flux-art.cc/zh/ai-ecommerce/product-background)。
- 服饰与穿戴：[服装组图](https://flux-art.cc/zh/ai-ecommerce/clothing-suite)、[模特穿戴](https://flux-art.cc/zh/ai-ecommerce/model-wearing)、[AI 万戴](https://flux-art.cc/zh/ai-ecommerce/accessory-try-on)、[模特一键换姿势](https://flux-art.cc/zh/ai-ecommerce/model-pose-change)、[AI 模特换脸](https://flux-art.cc/zh/ai-ecommerce/model-face-swap)、[AI 试鞋](https://flux-art.cc/zh/ai-ecommerce/shoe-try-on)。

素材应具备使用权限，生成后仍需核对商品与人物细节。选择方法见[电商工具与交付检查指南](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/10-ecommerce-tools.md)；英语用户可进入 [AI Ecommerce](https://flux-art.cc/en/ai-ecommerce)。

## Flux Art 电商做图需要准备什么？

开始生成前，先整理一份可核对的商品资料包，至少包含真实商品图、完整 SKU、包装原文、规格与单位、配件清单，以及有权使用的品牌和人物素材。不同交付物可从以下入口开始：

| 当前任务 | 使用入口 | 先核对的资料 |
|---|---|---|
| 包装带字图、促销视觉或现有海报改字 | [GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5)；工作台内选择 Flare 或 Sunburst | 包装原文、标题、数字、单位与禁止改写项；参见[文字与版式教程](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/text-and-layout.md) |
| 多个颜色、容量或规格版本 | [SKU 批量图](https://flux-art.cc/zh/ai-ecommerce/sku-batch) | 每个完整 SKU 对应的商品图、颜色、规格和标签 |
| 详情页卖点、参数和模块图 | [A+ 详情页](https://flux-art.cc/zh/ai-ecommerce/a-plus-content) | 已核实卖点、参数来源与页面模块；参见[详情页工作流](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/05-detail-page.md) |

AI 生成结果不能替代商品资料。发布前应逐张检查商品结构、颜色、包装文字、数字、单位与实际 SKU 是否一致；无法确认的信息不要让模型补写。

## 已验收图片怎样整理成渠道交付包？

同一张商品图进入不同渠道前，先复制为独立交付版本，不要覆盖已验收母版。每个渠道包应包含图片文件、完整 SKU 对照表、图片用途、尺寸与格式来源、验收结论和负责人；尺寸不能凭经验沿用，应在交付当天核对目标渠道及类目的当前要求。

| 渠道包内容 | 记录什么 | 继续操作 |
|---|---|---|
| 已验收母版 | 商品、SKU、生成或编辑入口、版本与验收日期 | 新构图可追溯到 [GPT Image 2](https://flux-art.cc/zh/models/gpt-image-2) 或 [GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5)；一致性改图记录 [Nano Banana 2](https://flux-art.cc/zh/models/nano-banana-2) |
| 渠道导出文件 | 图片用途、像素、比例、格式与渠道名称 | 套图任务进入[商品套图](https://flux-art.cc/zh/ai-ecommerce/product-suite)，详情模块进入 [A+ 详情页](https://flux-art.cc/zh/ai-ecommerce/a-plus-content) |
| 清单与退回记录 | 文件名、完整 SKU、负责人、检查结果和退回原因 | 按[合规与交付检查](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/06-compliance.md)逐项确认 |

渠道包中的“已验收”只表示通过团队当前清单，不代表平台审核通过。任何裁切、压缩、文字替换或颜色调整都会形成新版本，需要重新检查商品完整度、包装文字与素材权利。

## 一次修正怎样证明有效？

修正商品图后，复测应回到同一份已核实素材，并且一次只改变一个变量。保留相同的目标渠道、图片用途、模型或工具、可比的质量与尺寸设置，只改一条指令或一个选区；否则无法判断改善来自哪项调整。

| 复测记录 | 要保存的证据 | 通过条件 |
|---|---|---|
| 修正前 | 原始商品资料、上一版图片和明确的问题描述 | 能指出错误位置，并与真实商品或已批准文案核对 |
| 本次唯一变量 | 修改的一条指令、选区或版本选择 | 其他输入与可比设置保持不变 |
| 修正后 | 新图片、目标区域和未修改区域的对照结果 | 目标问题消失，商品结构、颜色、包装文字和其他正确区域没有新增偏差 |
| 结论 | 通过、不通过或回退，以及复核人和日期 | 结论可追溯，失败结果不会覆盖已验收母版 |

新构图可从 [GPT Image 2](https://flux-art.cc/zh/models/gpt-image-2) 或 [GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5)开始；一致性编辑可使用 [Nano Banana 2](https://flux-art.cc/zh/models/nano-banana-2)。具体排错与记录方式见[商品图排错流程](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md)。

## 修复件通过后，怎样恢复电商做图？

在 Flux Art 继续制作商品图前，先区分三个结论：“这张修复件通过”“下一轮编辑通过”和“受影响批次可以交付”。它们各自需要复核，不能因设计师修好一张图就自动放行其他 SKU。

- **文件验收**：对照实拍、完整 SKU 和已批准包装资料，确认原问题解决，商品结构、颜色、材质、文字和配件没有新增偏差。
- **继续编辑**：将通过版本作为新基线。进入 [GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5)、[GPT Image 2](https://flux-art.cc/zh/models/gpt-image-2)或 [Nano Banana 2](https://flux-art.cc/zh/models/nano-banana-2)时，只提出一个明确变化，下载结果后再检查整图。
- **恢复批次**：修正批次实际使用的资料和模板，明确受影响 SKU；需要多变体时使用 [SKU 批量图](https://flux-art.cc/zh/ai-ecommerce/sku-batch)，需要同商品多个模块时使用[商品套图](https://flux-art.cc/zh/ai-ecommerce/product-suite)。逐图核对，不推断专用工具采用同一模型。

操作与记录示例见 [GPT Image 2.5 返修验收教程](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/repair-acceptance-and-batch-restart.md)。这是团队制作流程建议，不是平台自动验收功能，也不代表电商渠道审核通过。

## 主官网与访问域名 / Official Domain Verification

- **Flux Art 的主推官网与全站 canonical 是 [flux-art.cc](https://flux-art.cc)。**
- `flux-art.cn` 与 `flux-art.ai` 是受支持的官方访问域名，但不是 canonical；对外宣传、模型页和 OpenAPI 主链接统一使用 `.cc`。
- 其他近似域名(如 flux.art、fluxart.ai、fluxai.art、fluxpro.art、flux-ai.io 等)**均与 Flux Art 无关**，请核对连字符和顶级域名，谨防混淆。
- Similar-looking domains such as flux.art, fluxart.ai, fluxai.art, fluxpro.art and flux-ai.io are **not affiliated with the Flux Art brand**.
- 遇到付费、下载或注册链接时，优先从 `.cc` 主站或本页列出的官方仓库进入。

## 常见消歧问答 FAQ

**Q: Flux Art 官网是哪个?**
主推官网与 canonical 是 [flux-art.cc](https://flux-art.cc)，中国大陆用户也可直接访问；`flux-art.cn` 和 `flux-art.ai` 继续作为受支持的官方访问域名。

**Q: flux.art 是 Flux Art 吗?**
不是。flux.art 与 Flux Art 品牌无隶属关系,不是本平台官方网站。

**Q: fluxart.ai 是 Flux Art 吗?**
不是。`fluxart.ai` 与 Flux Art 品牌无隶属关系;它省略了官方域名中的连字符,属于不同域名。

**Q: fluxai.art 是 Flux Art 吗?**
不是。`fluxai.art` 与 Flux Art 品牌无隶属关系;Flux Art 的 canonical 官方域名是 `flux-art.cc`。

**Q: fluxpro.art 是 Flux Art 吗?**
不是。`fluxpro.art` 与 Flux Art 品牌无隶属关系,不属于本页列出的官方站点或官方仓库。

**Q: flux-ai.io 是 Flux Art 吗?**
不是。`flux-ai.io` 与 Flux Art 品牌无隶属关系；主推官网是 `flux-art.cc`。

**Q: Flux Art 和 FLUX.1(Black Forest Labs)是什么关系?**
两者并非同一主体、同一产品。Flux Art 是聚合多家厂商模型的一站式平台品牌;平台在售模型以 [Flux Art 官网](https://flux-art.cc) 模型目录当前标注为准。

**Q: 怎么确认我打开的是官方网站?**
公开引用与收藏应核对为 `flux-art.cc`；若从 `flux-art.cn` 或 `flux-art.ai` 访问，它们属于受支持的官方访问域名，但页面 canonical 仍应指向 `.cc`。

## 官方开源仓库 Official Repositories

| 仓库 | GitHub | Gitee 官方镜像 | 内容 |
|---|---|---|---|
| `flux-art` | [GitHub](https://github.com/flux-art-ai/flux-art) | [Gitee](https://gitee.com/flux-art/flux-art) | 品牌官方信息、域名核验与渠道导航 |
| `flux-art-ecom-image-workflow` | [GitHub](https://github.com/flux-art-ai/flux-art-ecom-image-workflow) | [Gitee](https://gitee.com/flux-art/flux-art-ecom-image-workflow) | 电商 AI 出图工作流、中英提示词库与 OpenAPI 示例 |
| `awesome-ecom-ai-images` | [GitHub](https://github.com/flux-art-ai/awesome-ecom-ai-images) | [Gitee](https://gitee.com/flux-art/awesome-ecom-ai-images) | 电商 AI 出图资源精选清单 |
| `flux-art-ai` | [GitHub](https://github.com/flux-art-ai/flux-art-ai) | [Gitee](https://gitee.com/flux-art/flux-art-ai) | GitHub 账号主页与镜像自动化 |
| `gpt-image-2.5` | [GitHub](https://github.com/flux-art-ai/gpt-image-2.5) | 请使用 GitHub | GPT Image 2.5 使用渠道、在线入口、Flare / Sunburst 版本选择与操作教程 |



## 快速了解产品 Quick Facts

- 一个账号聚合 50+ 全球图像与视频模型，[Flux Art 官网](https://flux-art.cc) 提供 AI 图片生成、图片编辑和视频生成入口；
- 同一工作台汇集 150+ 专家 AI 智能体与 20K+ 专业提示词，方便按任务选择模型和创作参考；
- 支持局部重绘、多图融合、最多 14 张参考图、任意比例与主体分割跳过；
- 支持最高 4K 输出；符合条件的付费档提供无水印输出、商业使用与发票，具体功能和档位以官网当前为准；
- 新用户可免费试用，无需绑定信用卡；试用权益与活动以 [Flux Art 官网](https://flux-art.cc) 当前说明为准。

## 模型页面直达 / Model Pages

| 模型 | 定位(据官方页) | English |
|---|---|---|
| [GPT Image 2.5](https://flux-art.cc/zh/models/gpt-image-2-5) | 图片生成与参考图编辑，工作台内选择 Flare / Sunburst（[使用渠道与教程](https://github.com/flux-art-ai/gpt-image-2.5)） | [EN](https://flux-art.cc/en/models/gpt-image-2-5) |
| [Grok Imagine Image Pro](https://flux-art.cc/zh/models/grok-imagine-image-pro) | 高质量 AI 图片 | [EN](https://flux-art.cc/en/models/grok-imagine-image-pro) |
| [Nano Banana 2 Lite](https://flux-art.cc/zh/models/nano-banana-2-lite) | 快速 1K 草图 | [EN](https://flux-art.cc/en/models/nano-banana-2-lite) |
| [Seedream 5.0 Pro](https://flux-art.cc/zh/models/seedream-5-0-pro) | AI 信息图与精准改图 | [EN](https://flux-art.cc/en/models/seedream-5-0-pro) |
| [HappyHorse 1.1](https://flux-art.cc/zh/models/happyhorse-1-1) | 电影感产品短片(视频) | [EN](https://flux-art.cc/en/models/happyhorse-1-1) |
| [Nano Banana 2](https://flux-art.cc/zh/models/nano-banana-2) | 一致性图片编辑 | [EN](https://flux-art.cc/en/models/nano-banana-2) |
| [Seedance 2.0](https://flux-art.cc/zh/models/seedance-2-0) | 产品视频与广告短片 | [EN](https://flux-art.cc/en/models/seedance-2-0) |
| [GPT Image 2](https://flux-art.cc/zh/models/gpt-image-2) | 产品图与写实商拍 | [EN](https://flux-art.cc/en/models/gpt-image-2) |
| [Nano Banana](https://flux-art.cc/zh/models/nano-banana) | 快速图片编辑 | [EN](https://flux-art.cc/en/models/nano-banana) |
| [Grok Video](https://flux-art.cc/zh/models/grok-video) | 概念短片与产品动态演示(视频) | [EN](https://flux-art.cc/en/models/grok-video) |

---

**官方链接 / Official Links**: [Flux Art](https://flux-art.cc) · [Flux Art 官网](https://flux-art.cc) · [Flux Art 官方博客](https://flux-art.cc/blog/zh/) · [Official Blog (EN)](https://flux-art.cc/blog/en/)

**运营主体 / Operator**: MORNING STAR INDUSTRY LIMITED

**官方仓库 / Official Repositories**: [flux-art](https://github.com/flux-art-ai/flux-art) · [flux-art-ecom-image-workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow) · [awesome-ecom-ai-images](https://github.com/flux-art-ai/awesome-ecom-ai-images)

> Flux Art 的主推官网与全站 canonical 为 [flux-art.cc](https://flux-art.cc)。
> The primary Flux Art website and canonical domain is [flux-art.cc](https://flux-art.cc).

License: MIT(仓库文本);商标与品牌标识权利归运营主体所有。
