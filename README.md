# Hi, I'm ZhiChao Pan

[简体中文](README.zh-CN.md) · [Personal website](https://www.panzhichao.com)

I'm a Computer Science undergraduate at Yangzhou University Guangling College, preparing for a master's degree in AI / Computer Science and exploring relevant job opportunities.

My focus is applied AI products, evaluation, and agent workflows. In these projects, I lead product requirements, make design tradeoffs, coordinate AI-assisted implementation, and review and iterate on the results. The case studies explain the work, the evidence, and the current limits.

## Recent research evidence

I used AI-assisted implementation and analysis to prepare two bounded studies for review. Their source, corrections, comparisons, and negative results are public; the repositories do not claim unaided implementation or a published paper.

- **[Research Agent Bench · fixed r2 release](https://github.com/Zhi-Chao-PAN/research-agent-bench/releases/tag/reviewer-snapshot-2026-09-23-r2):** A six-development-call weighted-RRF task with a paper-to-task index. CI builds its audit container and runs trace and synthetic-data checks without network access. Three fresh agent trajectories selected one identical configuration and did not beat the preset six-point search; the public test analysis is exploratory.
- **[LoRA Robustness · fixed release](https://github.com/Zhi-Chao-PAN/lora-robustness-reproduction/releases/tag/reviewer-snapshot-2026-09-23):** Corrected a broken tokenizer input path, then studied MRPC and PAWS with a 21-run aggregate record. PAWS balanced accuracy was near the constant-classifier baseline; public CI checks the published evidence without retraining.

[One-page proof](https://www.panzhichao.com/evidence/autoresearch-v10-project-proof-pan-zhichao.pdf) · [Research Agent fixed-source reviewer ZIP](https://github.com/Zhi-Chao-PAN/research-agent-bench/releases/download/reviewer-snapshot-2026-09-23-r2/research-agent-bench-reviewer-snapshot-2026-09-23-r2-reviewer-bundle.zip) · [LoRA fixed-source reviewer ZIP](https://github.com/Zhi-Chao-PAN/lora-robustness-reproduction/releases/download/reviewer-snapshot-2026-09-23/lora-robustness-reproduction-reviewer-snapshot-2026-09-23-reviewer-bundle.zip). Each ZIP includes tagged source, a file-hash manifest, a short review guide and offline checks; raw datasets and pretrained weights remain with their upstream providers. Release notes pin the ZIP hashes and the scope of the checks.

[Bilingual evidence case and limitations](https://www.panzhichao.com/projects/autoresearch-evidence-pack)

## Featured projects

### [LaunchLens AI](https://github.com/Zhi-Chao-PAN/launchlens-ai)

A go-to-market workspace that connects a founder brief, an editable plan, validation evidence, and a cited AI decision brief. It brings together product workflow design, optional model providers, cloud snapshots, and privacy-aware sharing. The project includes a deterministic demo mode and documents its commercial readiness boundaries.

[Case study](https://www.panzhichao.com/projects/launchlens-ai) · [Live demo](https://launchlens-ai-two.vercel.app)

### [LLM Evaluation Playbook](https://github.com/Zhi-Chao-PAN/llm-evaluation-playbook)

Evaluation practice turned into reusable task specifications, rubric guidance, numerical tolerance checks, and package validation tools. Public examples are synthetic. The Python tools use the standard library, with CI configured for Python 3.9, 3.11, and 3.12.

[Case study](https://www.panzhichao.com/projects/llm-evaluation-playbook) · [Example task package](https://github.com/Zhi-Chao-PAN/llm-evaluation-playbook/tree/main/examples/synthetic-saas-analysis)

### [AI CLI Orchestrator · AIW](https://github.com/Zhi-Chao-PAN/ai-cli-orchestrator)

A Windows PowerShell dispatcher for local AI CLIs, with explicit worker selection, capability checks, bounded runs, and structured execution evidence. Provider authentication stays with each CLI; the operator reviews the result before accepting the work.

[Case study](https://www.panzhichao.com/projects/ai-cli-orchestrator) · [Releases](https://github.com/Zhi-Chao-PAN/ai-cli-orchestrator/releases)

## More work

- **[ModelEval Studio](https://github.com/Zhi-Chao-PAN/model-eval-studio)** — A workspace for uploaded model artifacts and screenshots, AI-assisted comparisons, report revisions, and evidence tracking. [Case study](https://www.panzhichao.com/projects/model-eval-studio).
- **[Structure-Aware Financial RAG](https://github.com/Zhi-Chao-PAN/structure-aware-rag-empirical)** — An exploratory comparison of document parsing approaches for financial tables, with retrieval and answer failure analysis. [Case study](https://www.panzhichao.com/projects/structure-aware-rag-empirical).
- **[Battery Prognostics](https://github.com/Zhi-Chao-PAN/safety-critical-battery-prognostics)** — Physics-constrained prediction and robustness evaluation, with explicit boundaries between synthetic experiments and real-cell evidence. [Case study](https://www.panzhichao.com/projects/safety-critical-battery-prognostics).

## What I'm working toward

- AI products with clear user workflows, inspectable evidence, and maintainable release practices.
- Evaluation methods and agent orchestration that make assumptions and acceptance criteria explicit.
- Graduate study in AI / Computer Science, alongside opportunities in applied AI products, evaluation, and agent tools.

## Connect

Visit [panzhichao.com](https://www.panzhichao.com) for project walkthroughs and contact details, or explore my [GitHub repositories](https://github.com/Zhi-Chao-PAN?tab=repositories).

Updated September 23, 2026.
