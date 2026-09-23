# 你好，我是潘志超

[English](README.md) · [个人网站](https://www.panzhichao.com/zh)

我目前就读于扬州大学广陵学院计算机相关专业，正在准备 AI / 计算机方向的硕士升学，也关注相关求职机会。

我关注 AI 应用产品、模型评测和智能体工作流。在这些项目中，我主要负责产品需求、方案取舍、组织 AI 辅助实现，以及结果检查和迭代。项目案例会说明解决的问题、已有证据和当前边界。

## 近期研究证据

三个研究案例围绕任务构造、训练输入核查和公平实验对照展开，公开源码、纠错记录、结果与复核入口。实现与分析使用 AI 工具协作；本人已完成的操作在下方单独说明。

- **[Research Agent Bench · r2 固定快照](https://github.com/Zhi-Chao-PAN/research-agent-bench/releases/tag/reviewer-snapshot-2026-09-23-r2)**：将加权 RRF 选参做成最多六次开发反馈的任务，公开论文到任务的对照索引。CI 构建审计容器，并在断网运行阶段检查轨迹与虚构数据。三条新增代理轨迹选到同一配置，未胜过预设六点搜索；公开测试分析属于探索性结果。
- **[LoRA 鲁棒性 · 固定快照](https://github.com/Zhi-Chao-PAN/lora-robustness-reproduction/releases/tag/reviewer-snapshot-2026-09-23)**：纠正错误分词输入后，在 MRPC 与 PAWS 上做有 21 次运行汇总记录的实验。PAWS balanced accuracy 接近常量预测基线；公开 CI 核验发布证据，不重新训练。
- **[电池容量重建 · 固定协议与三种子结果](https://github.com/Zhi-Chao-PAN/safety-critical-battery-prognostics/tree/74953917964a52798b3c352564aadbcf68f4d912/experiments/logo_capacity_reconstruction)**：六电芯留一验证，三个训练种子，两模型共 36 条结果。在相同噪声和后处理下，PINN/LSTM 平均 RMSE 为 0.9814/0.2221 Ah，PINN 对初始化更敏感；两者的零向上跳变来自共同的单调后处理。输入包含已观测容量，因此结论限于重建/去噪。

其后 AI 代理按固定 BEIR 获取脚本在同机[复跑 r2 源码](https://github.com/Zhi-Chao-PAN/research-agent-bench/blob/bda86d3f5d48b4b9a7d12ca8913ffdf4c989a238/PUBLIC_BEIR_UPSTREAM_REPLAY_2026-09-23.md)。本地获取日志与重建的排名缓存支持有限范围的数值重复性，不是独立网络来源证明、盲测或跨机器验证。

与公开实验分开，我在 WSL 亲自对 3 查询、12 文档虚构开发夹具做了六次不同候选调用，记录事前假设，并自行写出六题方法初稿。六题初稿包含预写部分；该记录说明本人已完成的具体操作范围。

[四页研究项目作品集](https://www.panzhichao.com/evidence/autoresearch-v15-project-portfolio-pan-zhichao.pdf) · [研究代理固定源码审阅包](https://github.com/Zhi-Chao-PAN/research-agent-bench/releases/download/reviewer-snapshot-2026-09-23-r2/research-agent-bench-reviewer-snapshot-2026-09-23-r2-reviewer-bundle.zip) · [LoRA 固定源码审阅包](https://github.com/Zhi-Chao-PAN/lora-robustness-reproduction/releases/download/reviewer-snapshot-2026-09-23/lora-robustness-reproduction-reviewer-snapshot-2026-09-23-reviewer-bundle.zip)。两个 ZIP 均含固定标签源码、逐文件哈希清单、简短审阅指南和离线核验；原始数据与预训练权重仍须从上游获取。各 Release 说明列有 ZIP 哈希和核验范围。

[中英文项目证据与边界](https://www.panzhichao.com/zh/projects/autoresearch-evidence-pack)

## 重点项目

### [LaunchLens AI](https://github.com/Zhi-Chao-PAN/launchlens-ai)

把创业想法、可编辑的市场进入计划、验证证据和引用证据的 AI 决策简报串起来的工作台。项目涉及产品流程设计、可选模型接入、云端快照和保护隐私的分享。项目提供确定性的演示模式，并公开说明商业化准备情况。

[项目案例](https://www.panzhichao.com/zh/projects/launchlens-ai) · [在线演示](https://launchlens-ai-two.vercel.app)

### [LLM Evaluation Playbook](https://github.com/Zhi-Chao-PAN/llm-evaluation-playbook)

把评测实践整理为可复用的任务规格、评分标准指引、数值容差检查和题包校验工具。公开示例均为合成内容；Python 工具只使用标准库，CI 配置覆盖 Python 3.9、3.11 和 3.12。

[项目案例](https://www.panzhichao.com/zh/projects/llm-evaluation-playbook) · [示例题包](https://github.com/Zhi-Chao-PAN/llm-evaluation-playbook/tree/main/examples/synthetic-saas-analysis)

### [AI CLI Orchestrator · AIW](https://github.com/Zhi-Chao-PAN/ai-cli-orchestrator)

用于调度本地 AI CLI 的 Windows PowerShell 工具，提供显式工作节点选择、能力检查、有时限的执行和结构化执行记录。各 CLI 保留自己的登录方式，最终由操作者检查结果并决定是否验收。

[项目案例](https://www.panzhichao.com/zh/projects/ai-cli-orchestrator) · [发布版本](https://github.com/Zhi-Chao-PAN/ai-cli-orchestrator/releases)

## 其他项目

- **[ModelEval Studio](https://github.com/Zhi-Chao-PAN/model-eval-studio)**：围绕已上传的模型产物和截图，提供 AI 辅助对比、报告修订和证据追溯。[项目案例](https://www.panzhichao.com/zh/projects/model-eval-studio)。
- **[Structure-Aware Financial RAG](https://github.com/Zhi-Chao-PAN/structure-aware-rag-empirical)**：探索财务表格的文档解析方案，分析检索与回答中的失败案例。[项目案例](https://www.panzhichao.com/zh/projects/structure-aware-rag-empirical)。
- **[Battery Prognostics](https://github.com/Zhi-Chao-PAN/safety-critical-battery-prognostics)**：电池容量重建与物理约束机制审查，采用公平后处理、留一电芯和多种子对照。[项目案例](https://www.panzhichao.com/zh/projects/safety-critical-battery-prognostics)。

## 当前方向

- 完善 AI 产品的用户流程、结果证据和发布维护方式。
- 研究评测方法与智能体调度，让假设、限制和验收标准更清楚。
- 准备 AI / 计算机方向硕士升学，同时寻找 AI 应用产品、评测和智能体工具方向的工作机会。

## 联系

欢迎访问 [panzhichao.com](https://www.panzhichao.com/zh) 查看完整项目案例和联系方式，也可以浏览我的 [GitHub 仓库](https://github.com/Zhi-Chao-PAN?tab=repositories)。

更新于 2026 年 9 月 23 日。
