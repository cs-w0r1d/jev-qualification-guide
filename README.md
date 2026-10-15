# Jev：把 AI 判断接进程序

面向公司技术分享的中文互动网页，按约 20 分钟编排。资料核验日期：2026-10-15；计划分享日期：2026-10-16。

在线阅读：https://cs-w0r1d.github.io/jev-qualification-guide/

## 使用

- 打开 `index.html` 即可离线阅读，无需安装依赖。
- 网页包含直接翻页展示、章节导航、讲者备注和日常消息分类交互。
- 讲者备注、API 示例及资料来源均在网页内。
- 所有应用与数值为教学示例；消息分类演示使用预设答案。交互在本地运行，没有调用 Jev API 或 Laya，也不会上传材料。

## 内容

以 Jev 的使用方法为主线，共 12 页、约 20 分钟：定位与适用任务；Choice / Score / Noul；完整 HTTP 请求与程序接收结果；六个分类、分流、排序与检查场景；消息分类互动；接入评估；Laya 开源模型及本地 Python 调用；资料索引。

Laya 是独立开源项目，不是 TypeSafe 官方发布的 Jev 开源版。页面依据官方代码、模型卡及用户提供的知乎文章介绍其用途，明确性能测试条件和接口语义差异。

代码仅展示接口用法，未执行真实模型推理，不构成完整生产服务。Jev 示例固定稳定版 1.13.0，并注明 1.14.0 预览版及别名情况；Laya 示例固定 0.4.7。模型判断、概率与阈值需要按任务验证。网页未公开原始训练数据、商品编号、图片链接或内部标签表。

## 维护与发布

这是一个自包含的静态网页。GitHub Pages 使用本仓库 `main` 分支根目录，`.nojekyll` 禁用 Jekyll 处理。更新 `index.html` 并提交至 `main` 后，Pages 会重新发布。该项目使用 `/jev-qualification-guide/` 路径，与 `cs-w0r1d.github.io` 个人主页仓库独立。

本地预览：`python3 -m http.server 8080`，然后访问 `http://localhost:8080/`。

## 资料来源

网页各节提供对应来源及参考资料页，优先使用 TypeSafe AI 官方文档、Laya 官方仓库和模型卡。模型能力、版本和价格可能变化，请在正式接入前复查。

- https://typesafe.ai/blog/introducing-system-one-models-and-jev
- https://docs.typesafe.ai/introduction
- https://docs.typesafe.ai/models
- https://docs.typesafe.ai/confidence
- https://docs.typesafe.ai/model-jaggedness/jev-1.13
- https://docs.typesafe.ai/api
- https://docs.typesafe.ai/primitives
- https://github.com/NandhaKishorM/laya
- https://huggingface.co/convaiinnovations/laya
- https://huggingface.co/convaiinnovations/laya-multilingual
- https://pypi.org/project/laya/
- https://zhuanlan.zhihu.com/p/2085760548034167437

用户提供的中文入门参考：https://www.eigent.ai/zh-CN/blog/typesafe-ai-jev-system-one-models
