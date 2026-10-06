---
name: mi-product-site-spec
description: 根据小米有品产品站47张原始规范图，制作、还原或校对1080px商品长页，覆盖头图、主打卖点、正文、图形与数字ICON、多图、细节、参数、品牌、获奖和FAQ；明确区分正确模板与错误示范。当用户提到“小米产品站规范”“有品产品站”或要求按本批图排版时使用。不同来源的商城详情页或轮播图规范不自动套用本skill。
---

# 小米有品产品站设计规范

本 skill 根据所附的 47 张小米有品产品站规范图片整理。详细规则与原图副本均在技能内，可离线核查。按明确标注制作；错误示范用于排除错误做法，不能作为可复用的正确模板。

## 先确定本次模块

| 模块 | 必选性与顺序 | 读取的规范 |
|---|---|---|
| 全局画布、文字层级、证据优先级 | 全任务基础 | [foundations.md](references/foundations.md) |
| 头图 | 必选 | [hero-and-selling-points.md](references/hero-and-selling-points.md) |
| 主打卖点网格 | 必备，头图下；有价格模块则放价格模块下 | [hero-and-selling-points.md](references/hero-and-selling-points.md) |
| 买点/卖点正文 | 必备，按产品实际拆分 | [body-and-icons.md](references/body-and-icons.md) |
| 图形 ICON、数字 ICON | 按需随正文使用 | [body-and-icons.md](references/body-and-icons.md) |
| 多图展示 | 按需 | [multi-image.md](references/multi-image.md) |
| 细节展示 | 可选，宫格或横版 | [details-parameters-brand.md](references/details-parameters-brand.md) |
| 规格参数 | 必备，有且只有 1P | [details-parameters-brand.md](references/details-parameters-brand.md) |
| 品牌介绍 | 必备，固定放参数页下方 | [details-parameters-brand.md](references/details-parameters-brand.md) |
| 获奖标识 | 按需，只出现在正文 | [details-parameters-brand.md](references/details-parameters-brand.md) |
| 常见问题 | 本批未声明必备性或固定位置 | [faq.md](references/faq.md) |
| 错误示范及修正 | 做头图/卖点或全页走查时必读 | [anti-patterns.md](references/anti-patterns.md) |
| 原图与规则冲突 | 核查任意疑点时读取 | [evidence-notes.md](references/evidence-notes.md)、[source-index.md](references/source-index.md) |

只读此次涉及的模块。制作完整产品站页时读全部使用模块及错误示范；仅修改一个模块时保持范围内工作。用户明确选择、指定尺寸或指定另一套规范时遵从用户，并说明相对于本规范的变化，不擅自扩大任务。

## 执行方式

1. 先识别图的角色：规范总览、单独标注模板、成品对照、错误示范。所有原图的编号见来源索引。
2. 用 1080px 设计基准建立对应模块，选择一种合法版式，填入真实产品名称、卖点、参数、品牌与有效标识。图片中的鸡蛋、椅子、热水器等只是示例产品，不是固定内容。
3. 按局部标注设置字重、字号、行距、尺寸、边距、颜色与行数。通用字阶仅作默认参考；原图未给的值属于实施选择，不能冒充规范硬值。
4. 文字区保持干净，保证图文对比；禁止规则按作用范围执行。移除尺寸箭头、标注文字和安全区色块；不要把演示板拼成商品页面。
5. 按 [review-checklist.md](references/review-checklist.md) 校对。若需要精确还原，打开 `references/source-images/Sxx.jpg` 对照具体版式；密集歧义中文字可用参照字体的字形匹配方法核对；普通使用本 skill 不依赖额外 OCR 工具。

## 不可丢失的约束

- 头图名称与 slogan 各 1–2 行；logo 必须存在并位于安全区；slogan 不能用卖点列表样式。
- 主打卖点是独立网格。两行标题时全部格都两行且不配描述；标题加描述时均为一行。禁止混用行数与排版样式、单独改格高、背景跳色等，详见错误示范。
- 图形 ICON 每排 2–4 个、最多两排；两排数量一致；不能单个展示。图形ICON与下方说明沿中心轴居中；数字ICON说明与数字左对齐。
- 文字、图片和 FAQ 的安全区不同，不能把 80px、50px、100px 混为一个全局 margin。
- 参数只有一页，多 SKU 共享一个标题；品牌固定接在参数下方。
- 获奖标识放正文。米家接入标识、版本标签按头图专门规则安排；彩黑版与纯白版按背景选用。
- 字号与颜色绑定具体用途。禁止把通用示例变成“全站只能这些字号/五种颜色”的限制。

## 设计走查的输出

用“模块 / 问题 / 当前实测值 / 规范值 / 修正方法 / 来源编号”说明可确认的偏差。只对可测得的值写实测数字；原图或输入不够清晰时明确待核实。已符合的可用一句话概括；不要在商品成品内展示这些实施说明。

## 来源与冲突

原图文字数值比 JPEG 像素采样更可靠。具体模块标注优先于 S36 通用字阶示例。确有标注互相冲突时，按 [evidence-notes.md](references/evidence-notes.md) 保留两种证据及采用依据，不静默修正。S20/S21/S23 是含正确对照的错误示范板，不表示其中所有内容都禁止。

这是本批“产品站”规范；不自动混入其他 `mi-detail-page-spec` 的参数行距、品牌字号、轮播图等规则。本批没有完整价格模块规范，也没有 PC 网页导航或响应式断点规范；相应内容按用户需求另行设计。
