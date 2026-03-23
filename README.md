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
- [📈 Notable use cases and writeups](#-notable-use-cases-and-writeups)
- [📄 License](#-license)

## 🛠️ General-purpose descendants

- [uditgoenka/autoresearch](https://github.com/uditgoenka/autoresearch) - Claude Code skill that generalizes autoresearch into a reusable loop for software, docs, security, shipping, debugging, and other measurable goals.
- [leo-lilinxiao/codex-autoresearch](https://github.com/leo-lilinxiao/codex-autoresearch) - Codex-native autoresearch skill with resume support, lessons across runs, optional parallel experiments, and mode-specific workflows.
- [davebcn87/pi-autoresearch](https://github.com/davebcn87/pi-autoresearch) - `pi` extension plus dashboard for persistent experiment loops, live metrics, confidence tracking, and resumable autoresearch sessions.
- [drivelineresearch/autoresearch-claude-code](https://github.com/drivelineresearch/autoresearch-claude-code) - Claude Code plugin/skill port of `pi-autoresearch`, with a clean experiment-loop workflow and a concrete biomechanics case study.
- [greyhaven-ai/autocontext](https://github.com/greyhaven-ai/autocontext) - Closed-loop control plane for repeated agent improvement, with evaluation, persistent knowledge, staged validation, and optional distillation into cheaper local runtimes.
- [jmilinovich/goal-md](https://github.com/jmilinovich/goal-md) - Generalizes autoresearch into a `GOAL.md` pattern for repos where the agent must first construct a measurable fitness function before it can optimize.
- [mutable-state-inc/autoresearch-at-home](https://github.com/mutable-state-inc/autoresearch-at-home) - Collaborative fork of upstream autoresearch that adds experiment claiming, shared best-config syncing, hypothesis exchange, and swarm-style coordination across many single-GPU agents.

## 🔬 Research-agent systems

- [aiming-lab/AutoResearchClaw](https://github.com/aiming-lab/AutoResearchClaw) - End-to-end research pipeline that turns a topic into literature review, experiments, analysis, peer review, and paper drafts; broader than autoresearch, but clearly in the same lineage.
- [OpenRaiser/NanoResearch](https://github.com/OpenRaiser/NanoResearch) - End-to-end autonomous research engine that plans experiments, generates code, runs jobs locally or on SLURM, analyzes real results, and writes papers grounded in those outputs.
- [wanshuiyin/Auto-claude-code-research-in-sleep](https://github.com/wanshuiyin/Auto-claude-code-research-in-sleep) - Markdown-first research workflows for Claude Code and other agents, centered on autonomous literature review, experiments, paper iteration, and cross-model critique.
- [Sibyl-Research-Team/AutoResearch-SibylSystem](https://github.com/Sibyl-Research-Team/AutoResearch-SibylSystem) - Fully autonomous AI scientist built on Claude Code, with explicit AutoResearch lineage, multi-agent research iteration, GPU experiment execution, and a self-evolving outer loop.
- [eimenhmdt/autoresearcher](https://github.com/eimenhmdt/autoresearcher) - Early open-source package for automating scientific workflows, currently centered on literature-review generation with an ambition toward broader autonomous research.
- [hyperspaceai/agi](https://github.com/hyperspaceai/agi) - Distributed, peer-to-peer research network where autonomous agents run experiments, gossip findings, maintain CRDT leaderboards, and archive results to GitHub across multiple research domains.

## 💻 Platform ports and hardware forks

- [miolini/autoresearch-macos](https://github.com/miolini/autoresearch-macos) - Widely adopted macOS fork that adapts upstream autoresearch for Apple Silicon / MPS while preserving the original loop shape.
- [trevin-creator/autoresearch-mlx](https://github.com/trevin-creator/autoresearch-mlx) - MLX-native Apple Silicon port that keeps the upstream fixed-budget `val_bpb` loop while removing the PyTorch/CUDA dependency entirely.
- [jsegov/autoresearch-win-rtx](https://github.com/jsegov/autoresearch-win-rtx) - Windows-native RTX fork focused on consumer NVIDIA GPUs, with explicit VRAM floors and a practical desktop setup path.
- [iii-hq/n-autoresearch](https://github.com/iii-hq/n-autoresearch) - Multi-GPU autoresearch infrastructure with structured experiment tracking, adaptive search strategy, crash recovery, and queryable orchestration around the classic `train.py` loop.
- [lucasgelfond/autoresearch-webgpu](https://github.com/lucasgelfond/autoresearch-webgpu) - Browser/WebGPU port that lets agents generate training code, run experiments in-browser, and feed results back into the loop without a Python setup.

## 🎯 Domain-specific adaptations

- [mattprusak/autoresearch-genealogy](https://github.com/mattprusak/autoresearch-genealogy) - Applies the autoresearch pattern to genealogy, using structured prompts, archive guides, source checks, and vault workflows to iteratively expand and verify family-history research.
- [ArchishmanSengupta/autovoiceevals](https://github.com/ArchishmanSengupta/autovoiceevals) - Uses adversarial callers plus keep-or-revert prompt edits to harden voice AI agents across Vapi, Smallest AI, and ElevenLabs.
- [chrisworsey55/atlas-gic](https://github.com/chrisworsey55/atlas-gic) - Applies the autoresearch keep-or-revert loop to trading agents, optimizing prompts and portfolio orchestration against rolling Sharpe ratio instead of model loss.
- [RightNow-AI/autokernel](https://github.com/RightNow-AI/autokernel) - Applies the autoresearch loop to GPU kernel optimization: profile bottlenecks, edit one kernel, benchmark, keep or revert, repeat.
- [Rkcr7/autoresearch-sudoku](https://github.com/Rkcr7/autoresearch-sudoku) - Enhanced autoresearch workflow where an AI agent iteratively rewrites and benchmarks a Rust sudoku solver, ultimately beating leading human-built solvers on hard benchmark sets.

## 📈 Notable use cases and writeups

- **Shopify Liquid optimization** - Tobi Lütke shared an autoresearch-style optimization run on Shopify's Liquid engine, with public traces showing major parse/render speedups and allocation reductions. ([tweet](https://x.com/tobi/status/2032212531846971413), [PR with traces](https://github.com/Shopify/liquid/pull/2056))
- **Driveline baseball biomechanics** - Public autoresearch-style experiment loop for pitch-velocity prediction from biomechanics data, with large reported gains in model quality. ([tweet](https://x.com/drivelinekyle/status/2032242254035992610))
- **Tennis XGBoost prediction + reward hacking writeup** - Nick Oak documents an autoresearch-inspired loop for tennis match prediction, including where the optimization setup went wrong. ([blog](https://nickoak.com/posts/tennis-xgboost-autoresearch/))
- **Vesuvius Challenge ink detection swarm** - Multi-agent experimental loop applied to ancient-scroll ink detection, with a strong writeup on cross-scroll generalization improvements. ([blog](https://scrollprize.substack.com/p/we-are-cooking))
- **Earth system model optimization** - Hybrid workflow where an LLM proposes equation structures and a search process tunes parameters, showing how the autoresearch pattern extends into scientific modeling. ([tweet](https://x.com/devparagiri/status/2035075626273739068), [blog](https://paragiri.com/blog/2026/autoresearch-earth-system-models/))

<div align="center">

## Star History

<a href="https://www.star-history.com/?type=date&repos=alvinunreal%2Fawesome-autoresearch">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/image?repos=alvinunreal/awesome-autoresearch&type=date&theme=dark&legend=top-left" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/image?repos=alvinunreal/awesome-autoresearch&type=date&legend=top-left" />
   <img alt="Star History Chart" src="https://api.star-history.com/image?repos=alvinunreal/awesome-autoresearch&type=date&legend=top-left" />
 </picture>
</a>

## 📄 License

This list is released under [CC0-1.0](./LICENSE).
