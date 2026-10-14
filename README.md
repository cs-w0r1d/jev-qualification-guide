# Jev × 商家商品资质审核治理

面向公司技术分享的中文互动网页，按约 20 分钟编排。资料核验日期：2026-10-15；计划分享日期：2026-10-16。

在线阅读：https://cs-w0r1d.github.io/jev-qualification-guide/

## 使用

- 打开 `index.html` 即可离线阅读，无需安装依赖。
- 网页包含直接翻页展示、章节导航、讲者备注和日常消息分类交互。
- 讲者备注、API 示例及资料来源均在网页内。
- 业务案例为构造或改编的教学示例；消息分类演示使用预设答案。交互在本地运行，没有调用 Jev API，也不会上传材料。

## 内容

从资质审核中的“语义匹配”出发，解释 Jev 的 System One 定位、Choice / Score / Noul、概率与 confidence 的区别，展示 OCR、权威核验、硬规则、模型判断、人工复核之间的分工，并给出可评估的试点方案。

代码示例仅展示接口用法，不构成生产审核策略。业务规则、阈值和审核结论需要使用企业自己的政策与标注数据验证。网页未公开原始训练数据、商品编号、图片链接或完整内部标签表。第七节按团购训练任务的结构改编，原始标注未在此独立复核。

## 维护与发布

这是一个自包含的静态网页。GitHub Pages 使用本仓库 `main` 分支根目录，`.nojekyll` 禁用 Jekyll 处理。更新 `index.html` 并提交至 `main` 后，Pages 会重新发布。该项目使用 `/jev-qualification-guide/` 路径，与 `cs-w0r1d.github.io` 个人主页仓库独立。

本地预览：`python3 -m http.server 8080`，然后访问 `http://localhost:8080/`。

## 资料来源

网页各节提供对应来源及参考资料页，优先使用 TypeSafe AI 官方文档和原始研究论文。模型能力、版本和价格可能变化，请在正式接入前复查。

- https://typesafe.ai/blog/introducing-system-one-models-and-jev
- https://docs.typesafe.ai/introduction
- https://docs.typesafe.ai/models
- https://docs.typesafe.ai/confidence
- https://docs.typesafe.ai/model-jaggedness/jev-1.13
- https://docs.typesafe.ai/api
- https://arxiv.org/abs/2609.37647
- https://arxiv.org/abs/2609.31142

用户提供的中文入门参考：https://www.eigent.ai/zh-CN/blog/typesafe-ai-jev-system-one-models
