<div align="center">

# 🔬 Awesome Autoresearch

**A curated, high-signal index of autonomous improvement loops, research agents, and descendants inspired by** [**karpathy/autoresearch**](https://github.com/karpathy/autoresearch).

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](./CONTRIBUTING.md)
[![License: CC0-1.0](https://img.shields.io/badge/license-CC0--1.0-blue.svg?style=flat-square)](./LICENSE)

</div>

## Contents

- [🛠️ General-purpose descendants](#️-general-purpose-descendants)
- [🔬 Research-agent systems](#-research-agent-systems)
- [💻 Platform ports and hardware forks](#-platform-ports-and-hardware-forks)
- [🎯 Domain-specific adaptations](#-domain-specific-adaptations)
- [📊 Evaluation & benchmarks](#-evaluation--benchmarks)
- [📈 Notable use cases and writeups](#-notable-use-cases-and-writeups)
- [📚 Related resources](#-related-resources)
- [📄 License](#-license)

## 🛠️ General-purpose descendants

- [uditgoenka/autoresearch](https://github.com/uditgoenka/autoresearch) ![GitHub stars](https://img.shields.io/github/stars/uditgoenka/autoresearch?style=social) - Claude Code skill that generalizes autoresearch into a reusable loop for software, docs, security, shipping, debugging, and other measurable goals.
- [leo-lilinxiao/codex-autoresearch](https://github.com/leo-lilinxiao/codex-autoresearch) ![GitHub stars](https://img.shields.io/github/stars/leo-lilinxiao/codex-autoresearch?style=social) - Codex-native autoresearch skill with resume support, lessons across runs, optional parallel experiments, and mode-specific workflows.
- [supratikpm/gemini-autoresearch](https://github.com/supratikpm/gemini-autoresearch) ![GitHub stars](https://img.shields.io/github/stars/supratikpm/gemini-autoresearch?style=social) - Gemini CLI skill that generalises autoresearch to any measurable goal. Gemini-native: uses Google Search grounding as a live verification source inside the loop, true headless overnight mode via --yolo --prompt, and 1M token context. Also works in Antigravity IDE via .agents/skills/.
- [davebcn87/pi-autoresearch](https://github.com/davebcn87/pi-autoresearch) ![GitHub stars](https://img.shields.io/github/stars/davebcn87/pi-autoresearch?style=social) - `pi` extension plus dashboard for persistent experiment loops, live metrics, confidence tracking, and resumable autoresearch sessions.
- [drivelineresearch/autoresearch-claude-code](https://github.com/drivelineresearch/autoresearch-claude-code) ![GitHub stars](https://img.shields.io/github/stars/drivelineresearch/autoresearch-claude-code?style=social) - Claude Code plugin/skill port of `pi-autoresearch`, with a clean experiment-loop workflow and a concrete biomechanics case study.
- [greyhaven-ai/autocontext](https://github.com/greyhaven-ai/autocontext) ![GitHub stars](https://img.shields.io/github/stars/greyhaven-ai/autocontext?style=social) - Closed-loop control plane for repeated agent improvement, with evaluation, persistent knowledge, staged validation, and optional distillation into cheaper local runtimes.
- [jmilinovich/goal-md](https://github.com/jmilinovich/goal-md) ![GitHub stars](https://img.shields.io/github/stars/jmilinovich/goal-md?style=social) - Generalizes autoresearch into a `GOAL.md` pattern for repos where the agent must first construct a measurable fitness function before it can optimize.
- [mutable-state-inc/autoresearch-at-home](https://github.com/mutable-state-inc/autoresearch-at-home) ![GitHub stars](https://img.shields.io/github/stars/mutable-state-inc/autoresearch-at-home?style=social) - Collaborative fork of upstream autoresearch that adds experiment claiming, shared best-config syncing, hypothesis exchange, and swarm-style coordination across many single-GPU agents.
- [zkarimi22/autoresearch-anything](https://github.com/zkarimi22/autoresearch-anything) ![GitHub stars](https://img.shields.io/github/stars/zkarimi22/autoresearch-anything?style=social) - Generalizes autoresearch to **any measurable metric** — system prompts, API performance, landing pages, test suites, config tuning, SQL queries. "If you can measure it, you can optimize it."
- [Entrpi/autoresearch-everywhere](https://github.com/Entrpi/autoresearch-everywhere) ![GitHub stars](https://img.shields.io/github/stars/Entrpi/autoresearch-everywhere?style=social) - Cross-platform expansion that auto-detects hardware config and starts the loop. The "glue and generalization" half of autoresearch.
- [ShengranHu/ADAS](https://github.com/ShengranHu/ADAS) ![GitHub stars](https://img.shields.io/github/stars/ShengranHu/ADAS?style=social) - **Automated Design of Agentic Systems** — ICLR 2025. Meta-agents that invent novel agent architectures by programming them in code.
- [MaximeRobeyns/self_improving_coding_agent](https://github.com/MaximeRobeyns/self_improving_coding_agent) ![GitHub stars](https://img.shields.io/github/stars/MaximeRobeyns/self_improving_coding_agent?style=social) - **SICA**: Self-Improving Coding Agent that edits its own codebase. ICLR 2025 Workshop paper demonstrating scaffold-level self-improvement on coding benchmarks.
- [peterskoett/self-improving-agent](https://github.com/peterskoett/self-improving-agent) ![GitHub stars](https://img.shields.io/github/stars/peterskoett/self-improving-agent?style=social) - Alternative self-improving agent architecture with reflection and meta-learning cycles.
- [metauto-ai/HGM](https://github.com/metauto-ai/HGM) ![GitHub stars](https://img.shields.io/github/stars/metauto-ai/HGM?style=social) - **Huxley-Gödel Machine** for coding agents — applies self-improvement to SWE-bench performance via meta-level optimization.
- [gepa-ai/gepa](https://github.com/gepa-ai/gepa) ![GitHub stars](https://img.shields.io/github/stars/gepa-ai/gepa?style=social) - **GEPA (Genetic-Pareto)** — ICLR 2026 Oral. Reflective prompt evolution that outperforms RL (GRPO) on benchmarks. Optimizes any textual parameters against any metric using natural language reflection.
- [MrTsepa/autoevolve](https://github.com/MrTsepa/autoevolve) ![GitHub stars](https://img.shields.io/github/stars/MrTsepa/autoevolve?style=social) - GEPA-inspired autoresearch for self-play: mutate code strategies, evaluate head-to-head, rate with Elo/Bradley-Terry, branch from the Pareto front. Agent reads match traces to target mutations. Works as a Claude Code skill.
- [HKUDS/ClawTeam](https://github.com/HKUDS/ClawTeam) ![GitHub stars](https://img.shields.io/github/stars/HKUDS/ClawTeam?style=social) - Agent swarm intelligence for autoresearch — spawns parallel GPU research directions, distributes work across agents, aggregates results.
- [Orchestra-Research/AI-Research-SKILLs](https://github.com/Orchestra-Research/AI-Research-SKILLs) ![GitHub stars](https://img.shields.io/github/stars/Orchestra-Research/AI-Research-SKILLs?style=social) - Comprehensive skill library including autoresearch orchestration with two-loop architecture (inner optimization + outer synthesis).
- [WecoAI/aideml](https://github.com/WecoAI/aideml) ![GitHub stars](https://img.shields.io/github/stars/WecoAI/aideml?style=social) - **AIDE**: Tree-search ML engineering agent that autonomously improves model performance via iterative code generation and evaluation.
- [weco.ai](https://weco.ai) - **Weco**: Cloud platform for AIDE with observability, experiment tracking, and managed runs — brings the autoresearch loop into production.

## 🔬 Research-agent systems

- [aiming-lab/AutoResearchClaw](https://github.com/aiming-lab/AutoResearchClaw) ![GitHub stars](https://img.shields.io/github/stars/aiming-lab/AutoResearchClaw?style=social) - End-to-end research pipeline that turns a topic into literature review, experiments, analysis, peer review, and paper drafts; broader than autoresearch, but clearly in the same lineage.
- [OpenRaiser/NanoResearch](https://github.com/OpenRaiser/NanoResearch) ![GitHub stars](https://img.shields.io/github/stars/OpenRaiser/NanoResearch?style=social) - End-to-end autonomous research engine that plans experiments, generates code, runs jobs locally or on SLURM, analyzes real results, and writes papers grounded in those outputs.
- [wanshuiyin/Auto-claude-code-research-in-sleep](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep) ![GitHub stars](https://img.shields.io/github/stars/wanshuiyin/Auto-claude-code-research-in-sleep?style=social) - Markdown-first research workflows for Claude Code and other agents, centered on autonomous literature review, experiments, paper iteration, and cross-model critique.
- [Sibyl-Research-Team/AutoResearch-SibylSystem](https://github.com/Sibyl-Research-Team/AutoResearch-SibylSystem) ![GitHub stars](https://img.shields.io/github/stars/Sibyl-Research-Team/AutoResearch-SibylSystem?style=social) - Fully autonomous AI scientist built on Claude Code, with explicit AutoResearch lineage, multi-agent research iteration, GPU experiment execution, and a self-evolving outer loop.
- [eimenhmdt/autoresearcher](https://github.com/eimenhmdt/autoresearcher) ![GitHub stars](https://img.shields.io/github/stars/eimenhmdt/autoresearcher?style=social) - Early open-source package for automating scientific workflows, currently centered on literature-review generation with an ambition toward broader autonomous research.
- [hyperspaceai/agi](https://github.com/hyperspaceai/agi) ![GitHub stars](https://img.shields.io/github/stars/hyperspaceai/agi?style=social) - Distributed, peer-to-peer research network where autonomous agents run experiments, gossip findings, maintain CRDT leaderboards, and archive results to GitHub across multiple research domains.
- [SakanaAI/AI-Scientist](https://github.com/SakanaAI/AI-Scientist) ![GitHub stars](https://img.shields.io/github/stars/SakanaAI/AI-Scientist?style=social) - **The AI Scientist**: First comprehensive system for fully automatic scientific discovery. From idea generation to paper writing with minimal human supervision.
- [SakanaAI/AI-Scientist-v2](https://github.com/SakanaAI/AI-Scientist-v2) ![GitHub stars](https://img.shields.io/github/stars/SakanaAI/AI-Scientist-v2?style=social) - Workshop-level automated scientific discovery via agentic tree search. Removes template dependency from v1, generalizes across research domains.
- [HKUDS/AI-Researcher](https://github.com/HKUDS/AI-Researcher) ![GitHub stars](https://img.shields.io/github/stars/HKUDS/AI-Researcher?style=social) - NeurIPS 2025 paper. Full end-to-end research automation: hypothesis → experiments → manuscript → peer review. Production version at [novix.science](https://novix.science/chat).
- [openags/Auto-Research](https://github.com/openags/Auto-Research) ![GitHub stars](https://img.shields.io/github/stars/openags/Auto-Research?style=social) - **OpenAGS**: Orchestrates a team of AI agents across the full research lifecycle — lit review, hypothesis generation, experiments, manuscript writing, and peer review.
- [SamuelSchmidgall/AgentLaboratory](https://github.com/SamuelSchmidgall/AgentLaboratory) ![GitHub stars](https://img.shields.io/github/stars/SamuelSchmidgall/AgentLaboratory?style=social) - End-to-end autonomous research workflow: idea → literature review → experiments → report. Supports both autonomous and co-pilot modes.
- [AgentRxiv](https://agentrxiv.github.io/) - Collaborative autonomous research framework where agent laboratories share a preprint server to build on each other's work iteratively.
- [JinheonBaek/ResearchAgent](https://github.com/JinheonBaek/ResearchAgent) ![GitHub stars](https://img.shields.io/github/stars/JinheonBaek/ResearchAgent?style=social) - Iterative research idea generation over scientific literature with LLMs. Multi-agent review and feedback loops.
- [du-nlp-lab/MLR-Copilot](https://github.com/du-nlp-lab/MLR-Copilot) ![GitHub stars](https://img.shields.io/github/stars/du-nlp-lab/MLR-Copilot?style=social) - Autonomous ML research framework — generates ideas, implements experiments, analyzes results.
- [MASWorks/ML-Agent](https://github.com/MASWorks/ML-Agent) ![GitHub stars](https://img.shields.io/github/stars/MASWorks/ML-Agent?style=social) - Reinforcing LLM agents for autonomous ML engineering. Learns from trial and error to improve model performance.
- [PouriaRouzrokh/LatteReview](https://github.com/PouriaRouzrokh/LatteReview) ![GitHub stars](https://img.shields.io/github/stars/PouriaRouzrokh/LatteReview?style=social) - Low-code Python package for **automated systematic literature reviews** via AI-powered agents.
- [LitLLM/LitLLM](https://github.com/LitLLM/LitLLM) ![GitHub stars](https://img.shields.io/github/stars/LitLLM/LitLLM?style=social) - AI-powered literature review assistant using RAG for accurate, well-structured related-work sections in academic writing.
- [Agent Laboratory](https://agentlaboratory.github.io/) - Three-phase research pipeline: Literature Review → Experimentation → Report Writing, with specialized agents for each phase.
- [WecoAI/aideml](https://github.com/WecoAI/aideml) ![GitHub stars](https://img.shields.io/github/stars/WecoAI/aideml?style=social) - **AIDE**: AI-Driven Exploration — tree-search-based ML engineering agent that automates experiment design, code generation, and evaluation. Treats ML engineering as code optimization against any metric.

## 💻 Platform ports and hardware forks

- [miolini/autoresearch-macos](https://github.com/miolini/autoresearch-macos) ![GitHub stars](https://img.shields.io/github/stars/miolini/autoresearch-macos?style=social) - Widely adopted macOS fork that adapts upstream autoresearch for Apple Silicon / MPS while preserving the original loop shape.
- [trevin-creator/autoresearch-mlx](https://github.com/trevin-creator/autoresearch-mlx) ![GitHub stars](https://img.shields.io/github/stars/trevin-creator/autoresearch-mlx?style=social) - MLX-native Apple Silicon port that keeps the upstream fixed-budget `val_bpb` loop while removing the PyTorch/CUDA dependency entirely.
- [jsegov/autoresearch-win-rtx](https://github.com/jsegov/autoresearch-win-rtx) ![GitHub stars](https://img.shields.io/github/stars/jsegov/autoresearch-win-rtx?style=social) - Windows-native RTX fork focused on consumer NVIDIA GPUs, with explicit VRAM floors and a practical desktop setup path.
- [iii-hq/n-autoresearch](https://github.com/iii-hq/n-autoresearch) ![GitHub stars](https://img.shields.io/github/stars/iii-hq/n-autoresearch?style=social) - Multi-GPU autoresearch infrastructure with structured experiment tracking, adaptive search strategy, crash recovery, and queryable orchestration around the classic `train.py` loop.
- [lucasgelfond/autoresearch-webgpu](https://github.com/lucasgelfond/autoresearch-webgpu) ![GitHub stars](https://img.shields.io/github/stars/lucasgelfond/autoresearch-webgpu?style=social) - Browser/WebGPU port that lets agents generate training code, run experiments in-browser, and feed results back into the loop without a Python setup.
- [tonitangpotato/autoresearch-engram](https://github.com/tonitangpotato/autoresearch-engram) ![GitHub stars](https://img.shields.io/github/stars/tonitangpotato/autoresearch-engram?style=social) - Fork with **persistent cognitive memory** — frequency-weighted retrieval of cross-session knowledge for improved experiment continuity.
- **Colab/Kaggle T4 port** - Adapts autoresearch for free T4 GPUs (Google Colab / Kaggle) with zero cost and zero local setup. Key changes: Flash Attention 3 → PyTorch SDPA, removes H100-only kernel dependency. ([upstream issue #208](https://github.com/karpathy/autoresearch/issues/208))

## 🎯 Domain-specific adaptations

- [mattprusak/autoresearch-genealogy](https://github.com/mattprusak/autoresearch-genealogy) ![GitHub stars](https://img.shields.io/github/stars/mattprusak/autoresearch-genealogy?style=social) - Applies the autoresearch pattern to genealogy, using structured prompts, archive guides, source checks, and vault workflows to iteratively expand and verify family-history research.
- [ArchishmanSengupta/autovoiceevals](https://github.com/ArchishmanSengupta/autovoiceevals) ![GitHub stars](https://img.shields.io/github/stars/ArchishmanSengupta/autovoiceevals?style=social) - Uses adversarial callers plus keep-or-revert prompt edits to harden voice AI agents across Vapi, Smallest AI, and ElevenLabs.
- [chrisworsey55/atlas-gic](https://github.com/chrisworsey55/atlas-gic) ![GitHub stars](https://img.shields.io/github/stars/chrisworsey55/atlas-gic?style=social) - Applies the autoresearch keep-or-revert loop to trading agents, optimizing prompts and portfolio orchestration against rolling Sharpe ratio instead of model loss.
- [RightNow-AI/autokernel](https://github.com/RightNow-AI/autokernel) ![GitHub stars](https://img.shields.io/github/stars/RightNow-AI/autokernel?style=social) - Applies the autoresearch loop to GPU kernel optimization: profile bottlenecks, edit one kernel, benchmark, keep or revert, repeat.
- [Rkcr7/autoresearch-sudoku](https://github.com/Rkcr7/autoresearch-sudoku) ![GitHub stars](https://img.shields.io/github/stars/Rkcr7/autoresearch-sudoku?style=social) - Enhanced autoresearch workflow where an AI agent iteratively rewrites and benchmarks a Rust sudoku solver, ultimately beating leading human-built solvers on hard benchmark sets.

## 📊 Evaluation & benchmarks

- [snap-stanford/MLAgentBench](https://github.com/snap-stanford/MLAgentBench) ![GitHub stars](https://img.shields.io/github/stars/snap-stanford/MLAgentBench?style=social) - Benchmark suite for evaluating AI agents on ML experimentation tasks. 13 tasks from CIFAR-10 to BabyLM.
- [openai/mle-bench](https://github.com/openai/mle-bench) ![GitHub stars](https://img.shields.io/github/stars/openai/mle-bench?style=social) - OpenAI's benchmark for measuring how well AI agents perform at ML engineering.
- [chchenhui/mlrbench](https://github.com/chchenhui/mlrbench) ![GitHub stars](https://img.shields.io/github/stars/chchenhui/mlrbench?style=social) - MLR-Bench: Evaluating AI agents on open-ended ML research. 201 tasks from NeurIPS/ICLR/ICML workshops.
- [gersteinlab/ML-Bench](https://github.com/gersteinlab/ML-Bench) ![GitHub stars](https://img.shields.io/github/stars/gersteinlab/ML-Bench?style=social) - Evaluates LLMs and agents for ML tasks on repository-level code.
- [THUDM/AgentBench](https://github.com/THUDM/AgentBench) ![GitHub stars](https://img.shields.io/github/stars/THUDM/AgentBench?style=social) - Comprehensive benchmark for LLM-as-Agent evaluation across 8 distinct environments. ICLR 2024.

## 📈 Notable use cases and writeups

- **Shopify Liquid optimization** - Tobi Lütke shared an autoresearch-style optimization run on Shopify's Liquid engine, with public traces showing major parse/render speedups and allocation reductions. ([tweet](https://x.com/tobi/status/2032212531846971413), [PR with traces](https://github.com/Shopify/liquid/pull/2056))
- **Driveline baseball biomechanics** - Public autoresearch-style experiment loop for pitch-velocity prediction from biomechanics data, with large reported gains in model quality. ([tweet](https://x.com/drivelinekyle/status/2032242254035992610))
- **Tennis XGBoost prediction + reward hacking writeup** - Nick Oak documents an autoresearch-inspired loop for tennis match prediction, including where the optimization setup went wrong. ([blog](https://nickoak.com/posts/tennis-xgboost-autoresearch/) · [repo](https://github.com/buildoak/tennis-xgboost-autoresearch) · [gamed branch](https://github.com/buildoak/tennis-xgboost-autoresearch/tree/archived/gamed-iterations))
- **Vesuvius Challenge ink detection swarm** - Multi-agent experimental loop applied to ancient-scroll ink detection, with a strong writeup on cross-scroll generalization improvements. ([blog](https://scrollprize.substack.com/p/we-are-cooking))
- **Earth system model optimization** - Hybrid workflow where an LLM proposes equation structures and a search process tunes parameters, showing how the autoresearch pattern extends into scientific modeling. ([tweet](https://x.com/devparagiri/status/2035075626273739068), [blog](https://paragiri.com/blog/2026/autoresearch-earth-system-models/))
- **The Agentic Researcher** - Paper: "A Practical Guide to AI-Assisted Research in Mathematics and Machine Learning." Cites autoresearch as the canonical example of automated ML experiment pipelines. ([arxiv 2603.15914](https://arxiv.org/html/2603.15914))
- **Scaling Autoresearch to GPU Clusters** - SkyPilot blog on running autoresearch on H100/H200 clusters with cloud orchestration. ([SkyPilot Blog](https://blog.skypilot.co/scaling-autoresearch/))
- **Self-Improving Coding Agents** - Addy Osmani's practical guide to setting up self-improving agent loops with Claude Code. ([article](https://addyosmani.com/blog/self-improving-agents/))
- **autoresearch@home: Distributed AI Research** - SETI@home model applied to autoresearch — contribute GPU time to collective model optimization. ([Ensue Blog](https://ensue.dev/blog/autoresearch-at-home/))
- **Claude Code + AutoResearch for Self-Improving Skills** - MindStudio guide to building self-improving AI skills using Claude Code with autoresearch patterns. ([article](https://www.mindstudio.ai/blog/claude-code-autoresearch-self-improving-skills))
- **100 ML Experiments Overnight** - Particula technical breakdown with domain-agnostic fork applications. ([article](https://particula.tech/blog/karpathy-autoresearch-autonomous-ml-experiments))
- **PM's Guide to Autoresearch** - Product manager's guide covering setup, community forks, and real-world applications. ([article](https://www.news.aakashg.com/p/autoresearch-guide-for-pms))
- **Autoresearch 101 Builder's Playbook** - Substack deep-dive on applying autoresearch patterns to prompts, agents, and workflows with concrete examples. ([article](https://sidsaladi.substack.com/p/autoresearch-101-builders-playbook))
- **Kingy AI Technical Breakdown** - Detailed technical walkthrough of the autoresearch loop architecture, mutation operators, and fitness function design. ([article](https://kingy.ai/ai/autoresearch-karpathys-minimal-agent-loop-for-autonomous-llm-experimentation/))
- **Fortune Feature** - Business and industry context on why autoresearch matters for the future of autonomous AI agents. ([article](https://fortune.com/2026/03/17/andrej-karpathy-loop-autonomous-ai-agents-future/))

## 📚 Related resources

Curated lists and paper collections for AI agents, autonomous systems, and automated research:

- [ai-agents-2030/awesome-deep-research-agent](https://github.com/ai-agents-2030/awesome-deep-research-agent) ![GitHub stars](https://img.shields.io/github/stars/ai-agents-2030/awesome-deep-research-agent?style=social) - Curated list of deep research agent papers and systems.
- [YoungDubbyDu/LLM-Agent-Optimization](https://github.com/YoungDubbyDu/LLM-Agent-Optimization) ![GitHub stars](https://img.shields.io/github/stars/YoungDubbyDu/LLM-Agent-Optimization?style=social) - Papers on LLM agent optimization methods.
- [VoltAgent/awesome-ai-agent-papers](https://github.com/VoltAgent/awesome-ai-agent-papers) ![GitHub stars](https://img.shields.io/github/stars/VoltAgent/awesome-ai-agent-papers?style=social) - Curated AI agent papers from 2026 — agent engineering, memory, evaluation, workflows, and autonomous systems.
- [masamasa59/ai-agent-papers](https://github.com/masamasa59/ai-agent-papers) ![GitHub stars](https://img.shields.io/github/stars/masamasa59/ai-agent-papers?style=social) - AI agent research papers updated biweekly via automated arxiv search with curated selection.
- [tmgthb/Autonomous-Agents](https://github.com/tmgthb/Autonomous-Agents) ![GitHub stars](https://img.shields.io/github/stars/tmgthb/Autonomous-Agents?style=social) - Autonomous agents research papers, updated daily.
- [HKUST-KnowComp/Awesome-LLM-Scientific-Discovery](https://github.com/HKUST-KnowComp/Awesome-LLM-Scientific-Discovery) ![GitHub stars](https://img.shields.io/github/stars/HKUST-KnowComp/Awesome-LLM-Scientific-Discovery?style=social) - EMNLP 2025 survey on LLMs in scientific discovery.
- [openags/Awesome-AI-Scientist-Papers](https://github.com/openags/Awesome-AI-Scientist-Papers) ![GitHub stars](https://img.shields.io/github/stars/openags/Awesome-AI-Scientist-Papers?style=social) - Collection of AI Scientist / Robot Scientist papers.
- [agenticscience.github.io](https://agenticscience.github.io/) - Survey: "From AI for Science to Agentic Science: A Survey on Autonomous Scientific Discovery."
- [dspy.ai/GEPA](https://dspy.ai/api/optimizers/GEPA/overview/) - DSPy integration of GEPA reflective prompt optimizer for compound AI systems.
- [OpenAI Cookbook: Self-Evolving Agents](https://developers.openai.com/cookbook/examples/partners/self_evolving_agents/autonomous_agent_retraining) - Cookbook for autonomous agent retraining using GEPA-style reflective evolution.
- [WecoAI/awesome-autoresearch](https://github.com/WecoAI/awesome-autoresearch) ![GitHub stars](https://img.shields.io/github/stars/WecoAI/awesome-autoresearch?style=social) - Curated list of AutoResearch use cases with verifiable traces and progress charts, organized by domain (LLM training, GPU kernels, voice agents, trading, etc.).

<div align="center">

## Star History

<a href="https://www.star-history.com/?type=date&repos=alvinunreal%2Fawesome-autoresearch">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/image?repos=alvinunreal%2Fawesome-autoresearch&type=date&theme=dark&legend=top-left" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/image?repos=alvinunreal%2Fawesome-autoresearch&type=date&legend=top-left" />
   <img alt="Star History Chart" src="https://api.star-history.com/image?repos=alvinunreal%2Fawesome-autoresearch&type=date&legend=top-left" />
 </picture>
</a>

## 📄 License

This list is released under [CC0-1.0](./LICENSE).
