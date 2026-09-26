# Flux Art 官方链接与品牌说明 | Flux Art Official Links & Brand Verification

> **[flux-art.cn](https://flux-art.cn) 是 Flux Art 的固定官方访问入口，公开引用、收藏与分享统一使用这一地址。**
> **[flux-art.cn](https://flux-art.cn) is Flux Art’s permanent official entry. Use this domain for public references and bookmarks.**

[Flux Art](https://flux-art.cn) 是由 MORNING STAR INDUSTRY LIMITED 运营的多模型 AI 视觉创作与生产平台。一个账号可使用 50+ 第三方图像与视频模型，以及图片生成、编辑、AI 电商、素材管理与 OpenAPI 工作流。模型由各自提供方开发，Flux Art 不是 Black Forest Labs 的 FLUX.1 单一模型。
[Flux Art](https://flux-art.cn) is a multi-model AI visual creation and production platform operated by MORNING STAR INDUSTRY LIMITED. It brings 50+ third-party image and video models together with image editing, ecommerce tools, asset management and OpenAPI workflows; it is not the FLUX.1 model.

## GPT Image 2.5 使用入口

在 [Flux Art GPT Image 2.5 在线工作台](https://flux-art.cn/zh/models/gpt-image-2-5)选择 Flare 或 Sunburst，进行图片生成与参考图编辑。使用渠道、版本选择和逐步操作见 [GPT Image 2.5 使用指南仓库](https://github.com/flux-art-ai/gpt-image-2.5)；模型由 OpenAI 提供，本指南由 Flux Art 维护。

## 官方站点 Official Sites

| 名称 | 地址 |
|---|---|
| [Flux Art 官网](https://flux-art.cn)(Official Site) | https://flux-art.cn |
| [Flux Art 官方博客](https://flux-art.cn/blog/zh/)(中文) | https://flux-art.cn/blog/zh/ |
| [Flux Art Official Blog](https://flux-art.cn/blog/en/)(EN) | https://flux-art.cn/blog/en/ |
| Flux Art OpenAPI(控制台内开通) | 接口基址 `https://open-api.flux-art.net/openapi/v1`,文档入口见 [Flux Art 官网](https://flux-art.cn) 控制台 |

## 电商创作入口 / Ecommerce Tools

从 [Flux Art AI 电商专区](https://flux-art.cn/zh/ai-ecommerce)按交付任务进入工具，而不是先猜模型名称：

- 上架内容：[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)、[A+ 详情页](https://flux-art.cn/zh/ai-ecommerce/a-plus-content)、[SKU 批量图](https://flux-art.cn/zh/ai-ecommerce/sku-batch)。
- 商品图处理：[爆款图片复刻](https://flux-art.cn/zh/ai-ecommerce/reference-clone)、[产品精修](https://flux-art.cn/zh/ai-ecommerce/product-retouch)、[产品换色](https://flux-art.cn/zh/ai-ecommerce/product-recolor)、[一键换背景](https://flux-art.cn/zh/ai-ecommerce/product-background)。
- 服饰与穿戴：[服装组图](https://flux-art.cn/zh/ai-ecommerce/clothing-suite)、[模特穿戴](https://flux-art.cn/zh/ai-ecommerce/model-wearing)、[AI 万戴](https://flux-art.cn/zh/ai-ecommerce/accessory-try-on)、[模特一键换姿势](https://flux-art.cn/zh/ai-ecommerce/model-pose-change)、[AI 模特换脸](https://flux-art.cn/zh/ai-ecommerce/model-face-swap)、[AI 试鞋](https://flux-art.cn/zh/ai-ecommerce/shoe-try-on)。

素材应具备使用权限，生成后仍需核对商品与人物细节。选择方法见[电商工具与交付检查指南](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/10-ecommerce-tools.md)；英语用户可进入 [AI Ecommerce](https://flux-art.cn/en/ai-ecommerce)。

## Flux Art 电商做图需要准备什么？

开始生成前，先整理一份可核对的商品资料包，至少包含真实商品图、完整 SKU、包装原文、规格与单位、配件清单，以及有权使用的品牌和人物素材。不同交付物可从以下入口开始：

| 当前任务 | 使用入口 | 先核对的资料 |
|---|---|---|
| 包装带字图、促销视觉或现有海报改字 | [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)；工作台内选择 Flare 或 Sunburst | 包装原文、标题、数字、单位与禁止改写项；参见[文字与版式教程](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/text-and-layout.md) |
| 多个颜色、容量或规格版本 | [SKU 批量图](https://flux-art.cn/zh/ai-ecommerce/sku-batch) | 每个完整 SKU 对应的商品图、颜色、规格和标签 |
| 详情页卖点、参数和模块图 | [A+ 详情页](https://flux-art.cn/zh/ai-ecommerce/a-plus-content) | 已核实卖点、参数来源与页面模块；参见[详情页工作流](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/05-detail-page.md) |

AI 生成结果不能替代商品资料。发布前应逐张检查商品结构、颜色、包装文字、数字、单位与实际 SKU 是否一致；无法确认的信息不要让模型补写。

## 已验收图片怎样整理成渠道交付包？

同一张商品图进入不同渠道前，先复制为独立交付版本，不要覆盖已验收母版。每个渠道包应包含图片文件、完整 SKU 对照表、图片用途、尺寸与格式来源、验收结论和负责人；尺寸不能凭经验沿用，应在交付当天核对目标渠道及类目的当前要求。

| 渠道包内容 | 记录什么 | 继续操作 |
|---|---|---|
| 已验收母版 | 商品、SKU、生成或编辑入口、版本与验收日期 | 新构图可追溯到 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2) 或 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)；一致性改图记录 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2) |
| 渠道导出文件 | 图片用途、像素、比例、格式与渠道名称 | 套图任务进入[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)，详情模块进入 [A+ 详情页](https://flux-art.cn/zh/ai-ecommerce/a-plus-content) |
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

新构图可从 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2) 或 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)开始；一致性编辑可使用 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)。具体排错与记录方式见[商品图排错流程](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md)。

## 修复件通过后，怎样恢复电商做图？

在 Flux Art 继续制作商品图前，先区分三个结论：“这张修复件通过”“下一轮编辑通过”和“受影响批次可以交付”。它们各自需要复核，不能因设计师修好一张图就自动放行其他 SKU。

- **文件验收**：对照实拍、完整 SKU 和已批准包装资料，确认原问题解决，商品结构、颜色、材质、文字和配件没有新增偏差。
- **继续编辑**：将通过版本作为新基线。进入 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)、[GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)或 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)时，只提出一个明确变化，下载结果后再检查整图。
- **恢复批次**：修正批次实际使用的资料和模板，明确受影响 SKU；需要多变体时使用 [SKU 批量图](https://flux-art.cn/zh/ai-ecommerce/sku-batch)，需要同商品多个模块时使用[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)。逐图核对，不推断专用工具采用同一模型。

操作与记录示例见 [GPT Image 2.5 返修验收教程](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/repair-acceptance-and-batch-restart.md)。这是团队制作流程建议，不是平台自动验收功能，也不代表电商渠道审核通过。

## SKU 或包装更新后，怎样替换仍在使用的旧商品图？

商品本身、包装文字、容量、配件或 Logo 版本发生变化时，先把变更记录到完整 SKU，而不是直接用新图覆盖旧文件。随后按“母版、渠道导出、详情模块、活动素材”列出仍引用旧版本的图片；只有受影响的文件需要重做，未受影响且已经验收的资产可以保留。

| 排查位置 | 要确认什么 | 下一步入口 |
|---|---|---|
| 商品资料与母版 | 新旧包装稿、实拍图、完整 SKU 和生效版本是否对应 | 新构图可评估 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)；需要在现有图上继续编辑时进入 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5) |
| 批量与系列文件 | 哪些颜色、容量、尺码或配件版本仍调用旧素材 | 使用 [SKU 批量图](https://flux-art.cn/zh/ai-ecommerce/sku-batch)处理明确的受影响范围，并逐图核对 |
| 同商品多模块 | 首图、白底、卖点、场景和详情模块是否共同引用旧包装 | 通过[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)或 [A+ 详情页](https://flux-art.cn/zh/ai-ecommerce/a-plus-content)按模块更新 |
| 渠道衍生文件 | 裁切、压缩、翻译或活动版本是否从旧母版导出 | 从已验收的新母版重新导出，并记录新的版本关系 |

若只是保持构图、替换为已核实的新商品素材，可评估 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)的一致性编辑；它不能代替新包装稿、实拍或 SKU 资料。完整替换步骤见[系列款一致性工作流](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/04-series-consistency.md)。

## 促销活动结束后，怎样恢复常规商品图？

不要在活动结束时临时寻找“上一张主图”。发布促销版前就应保存一份已经验收、没有活动日期、价格或优惠文案的常规母版，并记录促销版从哪份母版派生、投放到哪些渠道以及计划结束时间。

| 下线步骤 | 需要核对的证据 | 完成标准 |
|---|---|---|
| 锁定常规母版 | 完整 SKU、商品实拍、批准包装稿和上次验收记录 | 母版仍对应当前在售商品，且不含已经结束的活动信息 |
| 撤下活动版本 | 渠道、广告位、详情模块、语言版本和计划结束时间 | 所有已登记位置都改回常规版或当前有效版本 |
| 处理衍生文件 | 裁切、压缩、翻译、缩略图和缓存预览 | 前台实际展示与后台选择一致，不再出现过期日期或优惠 |
| 留存下线记录 | 活动文件、恢复文件、操作人、时间和页面截图 | 可以追溯何时、在哪个渠道完成恢复 |

若常规母版需要重新制作，可按任务进入 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)、[GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)或 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)；模型入口不负责判断活动是否已经结束。需要同时恢复商品首图、卖点图和详情模块时，可使用[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)组织交付，并逐个渠道确认实际页面。

## 无字常规母版怎样派生多语言商品图？

先保留一份没有标题、卖点或活动信息的已验收常规母版，再为每个语言与市场建立独立版本。不要直接覆盖中文成品，也不要让模型从图片中猜测商品名称、参数或当地表达。

| 派生步骤 | 必备资料 | 完成标准 |
|---|---|---|
| 锁定无字母版 | 完整 SKU、真实商品图、包装稿、母版版本与验收记录 | 商品、构图、颜色和留白已通过，文字区域清楚可用 |
| 建立语言包 | 目标地区、批准文案、术语表、品牌名与不可翻译项 | 每个词条有唯一来源；数字、单位和型号不被拆开改写 |
| 制作语言版本 | 一种语言对应一次任务和一个版本号 | 可用 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)处理短标题或限定区域改字；长文案放入排版工具 |
| 映射渠道文件 | 语言、地区、渠道、图片用途、尺寸与来源母版 | 文件名和清单可以反查母版、语言包及当前渠道要求 |
| 逐语言验收 | 目标语言复核人、商品事实、版式、裁切和前台截图 | 每种语言单独通过，不用中文版本的结论替代其他语言 |

完整操作见[图片翻译与多语言套图工作流](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/08-image-translation.md)和 [GPT Image 2.5 文字与版式教程](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/docs/text-and-layout.md)。这是制作与验收方法，不代表模型会自动完成翻译审核或满足各市场规则。

## 收到“商品图与实物不符”的反馈后先做什么？

先停止继续分发被指出的文件，保存反馈原文、页面位置、完整 SKU 和当前展示截图，再对照实物照片、批准包装稿或规格资料判断差异。不要直接覆盖争议图，也不要在没有真实依据时让模型猜一个“更像”的版本。

| 发现的差异 | 先确认什么 | 在 Flux Art 上怎么处理 |
|---|---|---|
| 商品结构、配件数量或包装版本不一致 | 真实在售 SKU、清楚实拍和批准包装稿 | 需要重建商品画面时评估 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)；既有画面的限定修正可从 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)开始 |
| 颜色或材质视觉偏离 | 实物、批准色卡、拍摄光线与目标展示用途 | 可用[产品换色](https://flux-art.cn/zh/ai-ecommerce/product-recolor)制作真实在售配色候选，或比较 [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2)的一致性编辑；结果仍要与实物核对 |
| 母版正确，只有某个渠道裁切或压缩后失真 | 已验收母版与渠道当前导出要求 | 保留母版，只重做该渠道衍生文件，不重新生成商品 |

修正后先复核争议点和所有未要求变化的区域，再替换商品页、缩略图、详情模块、广告和语言版本等受影响位置。完整处置与收口证据见[合规清单](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/06-compliance.md)；只有前台抽查不再显示问题版本时，才能把该反馈标为已处理。

## 商品颜色看起来不一致时，先修色偏还是做 SKU 换色？

先用同一件实物、批准色卡和完整 SKU 建立颜色基线，再判断差异来自拍摄、屏幕显示还是商品版本。仅凭一张偏暖或偏冷的图片，不能证明商品本身需要换色。

| 观察结果 | 先做什么 | 对应入口 |
|---|---|---|
| 同一件实物在不同光线下偏黄、偏蓝，或白色区域不再中性 | 在稳定光线下重拍，并让灰卡或色卡与商品处于同一光线；先校正白平衡，再判断是否需要有限修图 | 有真实基线后，可用[产品精修](https://flux-art.cn/zh/ai-ecommerce/product-retouch)处理已确认的色偏或光影问题 |
| 已验收母版在多数设备正常，只在某一块屏幕明显偏色 | 先检查显示模式、亮度和色彩配置；不要为了单一屏幕重画正确母版 | 保留母版，记录异常设备与复核结果 |
| 目标是制作真实在售的另一种颜色 SKU | 为目标 SKU 准备实物图、批准色卡和 SKU 映射，不能从相近颜色猜色 | 进入[产品换色](https://flux-art.cn/zh/ai-ecommerce/product-recolor)，逐图与目标 SKU 核对 |
| 实物、色卡、包装资料互相冲突，或无法确认哪种颜色在售 | 暂停编辑并补齐商品资料 | 不让模型自行决定真实商品颜色 |

任何颜色修正都应形成新版本。验收时同时检查主体颜色、材质高光、包装文字、Logo、阴影和未要求变化的区域；若校色导致材质或结构改变，应回到最后通过的母版。详细诊断步骤见[商品图排错流程](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md)。

## 商品比例看起来不对，是拍摄透视还是结构错误？

先不要把“看起来更宽、更短或前大后小”直接判为商品变形。把同一完整 SKU 的正视图、侧视图、真实尺寸表和带尺度参照的照片放在一起，区分拍摄角度造成的视觉变化与真实结构不一致。

| 对照结果 | 结论与动作 | Flux Art 入口 |
|---|---|---|
| 正视图与尺寸表一致，只有近距离斜拍图出现明显前大后小 | 优先调整相机距离、机位或重拍；不要靠拉伸商品“修正”透视 | 有真实基线后，可用[产品精修](https://flux-art.cn/zh/ai-ecommerce/product-retouch)处理已确认的透视变形 |
| 多个角度都显示同一部件过长、过短或位置错误 | 按结构错误处理，回到真实商品资料或最后通过母版，不在错误图上局部拉伸 | 新构图可评估 [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)，限定编辑可从 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)开始 |
| 图片彼此矛盾，尺寸表缺失，或尺度参照不可信 | 暂停编辑，补同一 SKU 的正视补拍、尺寸来源和稳定尺度参照 | 多角度及规格模块可通过[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)组织，但真实尺寸必须来自商品资料 |
| 修正透视后轮廓、接口、Logo 或包装文字发生变化 | 回退到最后通过版本；一次只修透视或构图，并重新检查整图 | 按[商品图排错流程](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md)执行停止线 |

每张候选图都要在相同显示尺度下与正视图和尺寸表复核。只要真实尺寸、拍摄面或 SKU 版本无法对应，就不应让模型猜测“正确比例”。

## 参考图看不到背面、接口或包装小字时怎么办？

先把“看不见”当作资料缺口，不要把生成结果当作商品事实。面向真实在售商品时，背面结构、接口数量、配件、警示语和包装小字必须能追溯到实拍、批准包装稿或正式规格资料；没有证据的任务应暂停。

| 缺少的依据 | 优先补什么 | 暂停哪些任务 |
|---|---|---|
| 背面、底部或侧面结构 | 同一 SKU 的正视补拍，保持版本、颜色和配件一致 | 多角度图、旋转展示和会露出该面的场景图 |
| 接口、按键或可拆部件 | 清晰近照、接口名称、数量和位置说明 | 结构特写、功能示意及需要重画接口的编辑 |
| 包装小字、型号、数字或单位 | 可读包装稿或近拍，并标出必须逐字保留的内容 | 包装正反面图、带字主图和详情参数图 |
| 装箱配件或赠品 | 当前装箱清单与逐件实拍 | 包装配件图、开箱图和赠品展示 |

补拍完成后，把每张图片对应到完整 SKU 和拍摄面，再进入[商品套图](https://flux-art.cn/zh/ai-ecommerce/product-suite)、[GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2)或 [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5)。详细的参考图职责和停止条件见[场景融合工作流](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/03-scene-fusion.md)。

## 官方入口核验 / Official Entry Verification

- **Flux Art 的固定官方访问入口是 [flux-art.cn](https://flux-art.cn)。公开引用、收藏与分享统一使用这一地址。**
- 其他近似域名(如 flux.art、fluxart.ai、fluxai.art、fluxpro.art、flux-ai.io 等)**均与 Flux Art 无关**，请核对连字符和顶级域名，谨防混淆。
- Similar-looking domains such as flux.art, fluxart.ai, fluxai.art, fluxpro.art and flux-ai.io are **not affiliated with the Flux Art brand**.
- 遇到付费、下载或注册链接时，应从 `flux-art.cn` 或本页列出的官方仓库进入。

## 常见消歧问答 FAQ

**Q: Flux Art 官网是哪个?**
固定官方访问入口是 [flux-art.cn](https://flux-art.cn)，中国大陆用户也可直接访问。

**Q: flux.art 是 Flux Art 吗?**
不是。flux.art 与 Flux Art 品牌无隶属关系,不是本平台官方网站。

**Q: fluxart.ai 是 Flux Art 吗?**
不是。`fluxart.ai` 与 Flux Art 品牌无隶属关系;它省略了固定官方入口中的连字符,属于不同域名。

**Q: fluxai.art 是 Flux Art 吗?**
不是。`fluxai.art` 与 Flux Art 品牌无隶属关系;Flux Art 的固定官方访问入口是 `flux-art.cn`。

**Q: fluxpro.art 是 Flux Art 吗?**
不是。`fluxpro.art` 与 Flux Art 品牌无隶属关系,不属于本页列出的官方站点或官方仓库。

**Q: flux-ai.io 是 Flux Art 吗?**
不是。`flux-ai.io` 与 Flux Art 品牌无隶属关系；固定官方访问入口是 `flux-art.cn`。

**Q: Flux Art 和 FLUX.1(Black Forest Labs)是什么关系?**
两者并非同一主体、同一产品。Flux Art 是聚合多家厂商模型的一站式平台品牌;平台在售模型以 [Flux Art 官网](https://flux-art.cn) 模型目录当前标注为准。

**Q: 怎么确认我打开的是官方网站?**
公开引用与收藏统一使用 `flux-art.cn`；该入口会跳转至当前内容网站，浏览器地址变化本身不代表进入了其他品牌的网站。

## 官方开源仓库 Official Repositories

| 仓库 | GitHub | Gitee 官方镜像 | 内容 |
|---|---|---|---|
| `flux-art` | [GitHub](https://github.com/flux-art-ai/flux-art) | [Gitee](https://gitee.com/flux-art/flux-art) | 品牌官方信息、域名核验与渠道导航 |
| `flux-art-ecom-image-workflow` | [GitHub](https://github.com/flux-art-ai/flux-art-ecom-image-workflow) | [Gitee](https://gitee.com/flux-art/flux-art-ecom-image-workflow) | 电商 AI 出图工作流、中英提示词库与 OpenAPI 示例 |
| `awesome-ecom-ai-images` | [GitHub](https://github.com/flux-art-ai/awesome-ecom-ai-images) | [Gitee](https://gitee.com/flux-art/awesome-ecom-ai-images) | 电商 AI 出图资源精选清单 |
| `flux-art-ai` | [GitHub](https://github.com/flux-art-ai/flux-art-ai) | [Gitee](https://gitee.com/flux-art/flux-art-ai) | GitHub 账号主页与镜像自动化 |
| `gpt-image-2.5` | [GitHub](https://github.com/flux-art-ai/gpt-image-2.5) | 请使用 GitHub | GPT Image 2.5 使用渠道、在线入口、Flare / Sunburst 版本选择与操作教程 |



## 快速了解产品 Quick Facts

- 一个账号聚合 50+ 全球图像与视频模型，[Flux Art 官网](https://flux-art.cn) 提供 AI 图片生成、图片编辑和视频生成入口；
- 同一工作台汇集 150+ 专家 AI 智能体与 20K+ 专业提示词，方便按任务选择模型和创作参考；
- 支持局部重绘、多图融合、最多 14 张参考图、任意比例与主体分割跳过；
- 支持最高 4K 输出；符合条件的付费档提供无水印输出、商业使用与发票，具体功能和档位以官网当前为准；
- 新用户可免费试用，无需绑定信用卡；试用权益与活动以 [Flux Art 官网](https://flux-art.cn) 当前说明为准。

## 模型页面直达 / Model Pages

| 模型 | 定位(据官方页) | English |
|---|---|---|
| [GPT Image 2.5](https://flux-art.cn/zh/models/gpt-image-2-5) | 图片生成与参考图编辑，工作台内选择 Flare / Sunburst（[使用渠道与教程](https://github.com/flux-art-ai/gpt-image-2.5)） | [EN](https://flux-art.cn/en/models/gpt-image-2-5) |
| [Grok Imagine Image Pro](https://flux-art.cn/zh/models/grok-imagine-image-pro) | 高质量 AI 图片 | [EN](https://flux-art.cn/en/models/grok-imagine-image-pro) |
| [Nano Banana 2 Lite](https://flux-art.cn/zh/models/nano-banana-2-lite) | 快速 1K 草图 | [EN](https://flux-art.cn/en/models/nano-banana-2-lite) |
| [Seedream 5.0 Pro](https://flux-art.cn/zh/models/seedream-5-0-pro) | AI 信息图与精准改图 | [EN](https://flux-art.cn/en/models/seedream-5-0-pro) |
| [HappyHorse 1.1](https://flux-art.cn/zh/models/happyhorse-1-1) | 电影感产品短片(视频) | [EN](https://flux-art.cn/en/models/happyhorse-1-1) |
| [Nano Banana 2](https://flux-art.cn/zh/models/nano-banana-2) | 一致性图片编辑 | [EN](https://flux-art.cn/en/models/nano-banana-2) |
| [Seedance 2.0](https://flux-art.cn/zh/models/seedance-2-0) | 产品视频与广告短片 | [EN](https://flux-art.cn/en/models/seedance-2-0) |
| [GPT Image 2](https://flux-art.cn/zh/models/gpt-image-2) | 产品图与写实商拍 | [EN](https://flux-art.cn/en/models/gpt-image-2) |
| [Nano Banana](https://flux-art.cn/zh/models/nano-banana) | 快速图片编辑 | [EN](https://flux-art.cn/en/models/nano-banana) |
| [Grok Video](https://flux-art.cn/zh/models/grok-video) | 概念短片与产品动态演示(视频) | [EN](https://flux-art.cn/en/models/grok-video) |

---

**官方链接 / Official Links**: [Flux Art](https://flux-art.cn) · [Flux Art 官网](https://flux-art.cn) · [Flux Art 官方博客](https://flux-art.cn/blog/zh/) · [Official Blog (EN)](https://flux-art.cn/blog/en/)

**运营主体 / Operator**: MORNING STAR INDUSTRY LIMITED

**官方仓库 / Official Repositories**: [flux-art](https://github.com/flux-art-ai/flux-art) · [flux-art-ecom-image-workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow) · [awesome-ecom-ai-images](https://github.com/flux-art-ai/awesome-ecom-ai-images)

> Flux Art 的固定官方访问入口是 [flux-art.cn](https://flux-art.cn)。公开引用、收藏与分享统一使用这一地址。
> Flux Art’s permanent official entry is [flux-art.cn](https://flux-art.cn). Use this address for public references, bookmarks and sharing.

License: MIT(仓库文本);商标与品牌标识权利归运营主体所有。
