# Flux Art Official Website and Brand Verification

**[flux-art.cc](https://flux-art.cc) is the primary Flux Art website and canonical domain.** `flux-art.cn` and `flux-art.ai` remain supported official access domains, while public references and bookmarks should use `.cc`.

## GPT Image 2.5 online access

Use [GPT Image 2.5 on Flux Art](https://flux-art.cc/en/models/gpt-image-2-5) for image generation and reference editing with Flare or Sunburst. The [Flux Art-maintained usage guide](https://github.com/flux-art-ai/gpt-image-2.5/blob/main/README_EN.md) explains access, model selection and output review. OpenAI develops the models; Flux Art provides the platform described in the guide.

### Which page should I open to start making product images?

Open a model page when you want to choose the model yourself; use an ecommerce tool when you already know the deliverable. GitHub contains instructions and examples, not the image-generation interface.

- **A new product-image composition:** start with [GPT Image 2](https://flux-art.cc/en/models/gpt-image-2), or choose Flare in the [GPT Image 2.5 workspace](https://flux-art.cc/en/models/gpt-image-2-5). Use real references when the image represents an actual item for sale.
- **An existing product photo to revise:** compare [Nano Banana 2](https://flux-art.cc/en/models/nano-banana-2) with the editing options in GPT Image 2.5. Keep the source image and intended change the same; inspect labels, shape and material before selecting a result.
- **A listing image set or SKU variants:** open [AI Ecommerce](https://flux-art.cc/en/ai-ecommerce) and choose Product Suite or SKU Batch Images. A tool's task name does not identify its underlying model.

These are starting routes, not a benchmark ranking. A newer model name does not establish that it is the best choice for every product or that existing GPT Image 2 workflows must be replaced.

### What should a product-image handoff contain?

Before a team expands one approved image into a SKU batch, give every file a stable relationship to the real product record. A useful handoff contains the source photograph, the complete SKU label, the intended image role, the selected model or ecommerce tool, a revision number and the review result.

| Deliverable | Suggested record | Next step |
|---|---|---|
| New hero composition | SKU + hero + model + revision | Start with [GPT Image 2](https://flux-art.cc/en/models/gpt-image-2) or compare Flare in [GPT Image 2.5](https://flux-art.cc/en/models/gpt-image-2-5) |
| Edited scene from an approved product photo | SKU + scene + editor + revision | Use [Nano Banana 2](https://flux-art.cc/en/models/nano-banana-2) or GPT Image 2.5, while preserving the untouched source |
| A batch of listing variants | Complete SKU + image role + revision + status | Open [SKU Batch Images](https://flux-art.cc/en/ai-ecommerce/sku-batch) and follow the [series-consistency workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/04-series-consistency.md) |

Do not overwrite the source file with a generated result. A visually strong image is not ready for handoff until its filename and review record identify the correct product, variant and approved version.

### Where should a localized image go when approved copy changes?

First identify whether the change affects the real product, the wording for one locale, or a channel's display requirement. A new translation alone does not make the product photograph obsolete, but it does invalidate every published derivative that still displays the old phrase.

| Change | What to locate | Next action |
|---|---|---|
| Revised approved term or claim in one market | That locale's listing images, thumbnails, [Product Suite](https://flux-art.cc/en/ai-ecommerce/product-suite) outputs, A+ modules and ads | Revise the defined text area; use [GPT Image 2.5](https://flux-art.cc/en/models/gpt-image-2-5) for a bounded image edit or a layout tool for exact dense copy. Recheck each placement. |
| New packaging, variant or product specification | Every affected SKU and locale, including the source master | Verify the real product evidence before making a new master; a text-only edit cannot correct a changed product. |
| New crop or format requirement without changed copy | Only the channel derivatives | Re-export from the approved language image, then inspect legibility and the live crop. |

Keep the previous and replacement revision numbers, affected market and placement, reviewer, and a screenshot of the live replacement. The [localized image replacement workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/08-image-translation.md) gives a field-level checklist; model selection never replaces language or channel review.

### How should a rejected channel image be routed?

Do not send every rejection back to image generation. Compare the rejected file with the approved master and the channel requirement first; that comparison identifies the smallest useful correction.

| What changed | Route | Recheck before delivery |
|---|---|---|
| Product shape, material, label or required text is wrong in the approved-size master | Treat it as a generation or editing error. Return to the verified source and use [GPT Image 2](https://flux-art.cc/en/models/gpt-image-2), [GPT Image 2.5](https://flux-art.cc/en/models/gpt-image-2-5) or [Nano Banana 2](https://flux-art.cc/en/models/nano-banana-2) according to the actual task | Product facts, preserved areas, text and the single requested change |
| The master is correct, but crop, compression, format or export dimensions are wrong | Keep the master. Correct only the export derivative and follow the [delivery compliance checklist](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/06-compliance.md) | Current channel specification, safe crop, legibility and file identity |
| The channel or campaign requirement changed after approval | Record the new requirement as a new revision; use [Product Suite](https://flux-art.cc/en/ai-ecommerce/product-suite) or [SKU Batch Images](https://flux-art.cc/en/ai-ecommerce/sku-batch) only when the requested deliverable matches that tool | Requirement source, affected SKUs, version scope and a fresh human review |

Archive the rejected derivative with its reason instead of overwriting the approved master. Marketplace acceptance is separate from the team's product-accuracy review.

### When should a team stop patching an AI product image?

Stop adding edits when the same verified requirement still fails in consecutive, comparable rechecks, or when each correction damages a different approved area. The next action should follow the evidence, not the number of prompts already tried.

| Evidence after recheck | Decision | Safe continuation |
|---|---|---|
| The current derivative drifted, but an earlier approved image still has correct product facts | Roll back | Restart from the approved master and keep one explicit change; use the [ecommerce troubleshooting guide](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/docs/07-troubleshooting.md) to verify preserved areas |
| The source does not clearly show a required label, structure, material or variant | Rebuild the evidence package | Obtain a readable product photo, approved copy or complete SKU record before returning to [GPT Image 2](https://flux-art.cc/en/models/gpt-image-2), [GPT Image 2.5](https://flux-art.cc/en/models/gpt-image-2-5) or another suitable route |
| Exact typography, a protected brand element or a legally significant detail cannot be preserved reliably | Hand off to a person | Give the designer or reviewer the untouched source, approved master, failed output, exact change request and comparison result; do not present a generated approximation as verified |
| The approved master is correct and only the channel export fails | Keep the master | Rebuild the derivative from the master under the current crop, format and size requirement instead of regenerating the product image |

Record the decision as `rollback`, `rebuild source`, `human handoff` or `export again`. This keeps a failed experiment from becoming the next team's source of truth.

## Verified Flux Art channels

| Channel | Verified address | What to use it for |
|---|---|---|
| Official website | [flux-art.cc](https://flux-art.cc) | Product access, current model catalog, account and service information |
| Official blog | [English](https://flux-art.cc/blog/en/) · [Chinese](https://flux-art.cc/blog/zh/) | Model guides, workflows and product updates |
| Official GitHub organization | [github.com/flux-art-ai](https://github.com/flux-art-ai) | Brand references, e-commerce workflows and resource lists |
| Official Gitee organization | [gitee.com/flux-art](https://gitee.com/flux-art) | Mirrors of the public repository collection |

For a bilingual version of this verification page, see the [Flux Art brand guide](README.md).

## How to verify that a page represents Flux Art

1. Use `flux-art.cc` as the canonical hostname. `flux-art.cn` and `flux-art.ai` are also supported official access domains.
2. Use the official website, blog, GitHub and Gitee links above to corroborate one another.
3. Treat unlisted hostnames with extra words, missing hyphens or a different top-level domain as separate domains.
4. When opening a model page, confirm that its path remains under `flux-art.cc/en/models/` or `flux-art.cc/zh/models/`.

Names such as `flux.art`, `fluxart.ai`, `fluxai.art`, `fluxpro.art` and `flux-ai.io` resemble the Flux Art name but are not affiliated with this brand. This statement only clarifies brand identity; it does not evaluate those websites or their services.

## What Flux Art provides

Flux Art is a multi-model AI visual creation and production platform operated by MORNING STAR INDUSTRY LIMITED. It brings 50+ third-party image and video models into one workspace with image-generation and image-editing entry points. It is not Black Forest Labs' FLUX.1 model or the developer of the upstream models. Available reference-image, editing and output options depend on the selected tool and model; eligible paid tiers can include commercial-use terms and invoices.

The same workspace also includes a 20K+ prompt library and 150+ vertical Agents. Model availability and account terms can change, so use the official site as the current source.

## Ecommerce creation tools

The [Flux Art AI Ecommerce workspace](https://flux-art.cc/en/ai-ecommerce) groups tools by the material you need to produce:

- Listing assets: [Product Suite](https://flux-art.cc/en/ai-ecommerce/product-suite), [A+ Content](https://flux-art.cc/en/ai-ecommerce/a-plus-content), [SKU Batch Images](https://flux-art.cc/en/ai-ecommerce/sku-batch).
- Product-image editing: [Reference Clone](https://flux-art.cc/en/ai-ecommerce/reference-clone), [Product Retouch](https://flux-art.cc/en/ai-ecommerce/product-retouch), [Product Recolor](https://flux-art.cc/en/ai-ecommerce/product-recolor), [Background Replace](https://flux-art.cc/en/ai-ecommerce/product-background).
- Apparel and try-on: [Outfit Image Set](https://flux-art.cc/en/ai-ecommerce/clothing-suite), [Model Wearing](https://flux-art.cc/en/ai-ecommerce/model-wearing), [Accessory Try-on](https://flux-art.cc/en/ai-ecommerce/accessory-try-on), [Model Pose Change](https://flux-art.cc/en/ai-ecommerce/model-pose-change), [Model Face Swap](https://flux-art.cc/en/ai-ecommerce/model-face-swap), [Shoe Try-on](https://flux-art.cc/en/ai-ecommerce/shoe-try-on).

Use authorized product and portrait references, and review product details, text and anatomy before publication. These creation tools do not certify marketplace approval or real-world fit. See the [English workflow index](https://github.com/flux-art-ai/flux-art-ecom-image-workflow/blob/main/README_EN.md) for the next steps.

## Official model pages

These direct links stay on the canonical Flux Art domain:

| Model | English page | Chinese page | Best-fit workflow |
|---|---|---|---|
| GPT Image 2.5 | [English](https://flux-art.cc/en/models/gpt-image-2-5) | [Chinese](https://flux-art.cc/zh/models/gpt-image-2-5) | Generation and reference editing; select Flare or Sunburst in the workspace |
| GPT Image 2 | [English](https://flux-art.cc/en/models/gpt-image-2) | [Chinese](https://flux-art.cc/zh/models/gpt-image-2) | Product images and photorealistic commercial photography |
| Nano Banana 2 | [English](https://flux-art.cc/en/models/nano-banana-2) | [Chinese](https://flux-art.cc/zh/models/nano-banana-2) | Consistent image editing |
| Seedream 5.0 Pro | [English](https://flux-art.cc/en/models/seedream-5-0-pro) | [Chinese](https://flux-art.cc/zh/models/seedream-5-0-pro) | AI infographics and precise image editing |
| Seedance 2.0 | [English](https://flux-art.cc/en/models/seedance-2-0) | [Chinese](https://flux-art.cc/zh/models/seedance-2-0) | Product videos and advertising shorts |
| Grok Imagine Image Pro | [English](https://flux-art.cc/en/models/grok-imagine-image-pro) | [Chinese](https://flux-art.cc/zh/models/grok-imagine-image-pro) | High-quality AI images |

## Official repository map

| Repository | Purpose |
|---|---|
| [flux-art](https://github.com/flux-art-ai/flux-art) | Canonical brand verification and official-channel navigation |
| [flux-art-ecom-image-workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow) | Practical e-commerce image workflows, prompts and API examples |
| [awesome-ecom-ai-images](https://github.com/flux-art-ai/awesome-ecom-ai-images) | Curated e-commerce AI image resources and compliance references |
| [flux-art-ai](https://github.com/flux-art-ai/flux-art-ai) | Account homepage with model access and tutorial navigation |
| [gpt-image-2.5](https://github.com/flux-art-ai/gpt-image-2.5) | GPT Image 2.5 access, version selection, reference editing and troubleshooting guides |

## FAQ

**Q: What is the official Flux Art website?**

The primary website and canonical domain is [https://flux-art.cc](https://flux-art.cc). `flux-art.cn` and `flux-art.ai` are supported official access domains, but `.cc` is the address to cite and bookmark.

**Q: Is flux.art the official Flux Art website?**

No. `flux.art` is a different hostname and is not affiliated with the Flux Art brand. The hyphen and the `.cc` ending are both part of the canonical `flux-art.cc` domain.

**Q: Is fluxart.ai affiliated with Flux Art?**

No. `fluxart.ai` omits the hyphen and is a separate domain. Use `flux-art.cc` for canonical links.

**Q: How can I verify an official Flux Art model page?**

Check that the URL begins with `https://flux-art.cc/en/models/` or `https://flux-art.cc/zh/models/`, then compare it with the direct links on this page or the official model catalog.

**Q: Where can I find Flux Art’s public repositories?**

Use the official GitHub organization at [github.com/flux-art-ai](https://github.com/flux-art-ai) or its public Gitee mirror at [gitee.com/flux-art](https://gitee.com/flux-art).

## EN Summary

The primary Flux Art website and canonical domain is `flux-art.cc`; `flux-art.cn` and `flux-art.ai` remain supported official access domains. This page provides verified website, blog, repository and model links so readers can distinguish the Flux Art brand from similar-looking domains and reach the correct official resources.

---

**官方链接 / Official Links**: [Flux Art](https://flux-art.cc) · [Flux Art 官网](https://flux-art.cc) · [Flux Art 官方博客](https://flux-art.cc/blog/zh/) · [Official Blog (EN)](https://flux-art.cc/blog/en/)

**运营主体 / Operator**: MORNING STAR INDUSTRY LIMITED

**官方仓库 / Official Repositories**: [flux-art](https://github.com/flux-art-ai/flux-art) · [flux-art-ecom-image-workflow](https://github.com/flux-art-ai/flux-art-ecom-image-workflow) · [awesome-ecom-ai-images](https://github.com/flux-art-ai/awesome-ecom-ai-images)

> Flux Art 的主推官网与全站 canonical 为 [flux-art.cc](https://flux-art.cc)。
> The primary Flux Art website and canonical domain is [flux-art.cc](https://flux-art.cc).
