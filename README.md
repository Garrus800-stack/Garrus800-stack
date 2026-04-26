# Daniel — `@Garrus800-stack`

**Solo architect of self-modifying AI systems.**
Building agents that read their own code, fix their own bugs, and evolve their own architecture.

![Profile views](https://komarev.com/ghpvc/?username=Garrus800-stack&style=flat-square&color=6c8cff&label=profile+views)

&nbsp;

[![Genesis Agent](https://img.shields.io/badge/Genesis_Agent-v7.4.7-6c8cff?style=for-the-badge&logo=electron&logoColor=white)](https://github.com/Garrus800-stack/genesis-agent)
[![Tests](https://img.shields.io/badge/tests-5716_passing-2da44e?style=for-the-badge)](https://github.com/Garrus800-stack/genesis-agent)
[![Fitness](https://img.shields.io/badge/architectural_fitness-127%2F130-2da44e?style=for-the-badge)](https://github.com/Garrus800-stack/genesis-agent)
[![Coverage](https://img.shields.io/badge/coverage-83%2F77%2F80-2da44e?style=for-the-badge)](https://github.com/Garrus800-stack/genesis-agent)

[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=000)](https://github.com/Garrus800-stack/genesis-agent)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)](https://github.com/Garrus800-stack/genesis-agent)
[![Electron](https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white)](https://github.com/Garrus800-stack/genesis-agent)
[![MCP](https://img.shields.io/badge/MCP-Protocol-8A2BE2?style=flat-square)](https://github.com/Garrus800-stack/genesis-agent)
[![Anthropic](https://img.shields.io/badge/Anthropic-D97757?style=flat-square)](https://github.com/Garrus800-stack/genesis-agent)
[![Ollama](https://img.shields.io/badge/Ollama-000?style=flat-square)](https://github.com/Garrus800-stack/genesis-agent)

---

<a href="https://github.com/Garrus800-stack"><img src="https://github-readme-stats.vercel.app/api?username=Garrus800-stack&show_icons=true&hide_border=true&title_color=6c8cff&icon_color=6c8cff&text_color=c2c0b6&bg_color=00000000&include_all_commits=true&count_private=true" height="165" alt="GitHub Stats" /></a>
<a href="https://github.com/Garrus800-stack"><img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Garrus800-stack&layout=compact&hide_border=true&title_color=6c8cff&text_color=c2c0b6&bg_color=00000000&langs_count=8" height="165" alt="Top Languages" /></a>

---

## Genesis Agent

A self-aware, self-modifying cognitive AI agent with a 12-phase boot system, hexagonal architecture, and organism substrate. It doesn't just use LLMs — it wraps them in 296 modules of self-verification, self-repair, causal reasoning, autonomous planning, and runtime self-modification with rollback.

```
296 source files · ~96k LOC · 5716 tests · 167 services
12 boot phases · 127/130 architectural fitness · coverage 83/77/80
16 hash-locked safety files · 302 late-bindings · 379 event types
Crash-safe sessions · Frontier-based memory · Heuristic self-scoring
Runtime-toggleable subsystems · i18n EN/DE
Runs on Claude, GPT-4, Qwen, DeepSeek, Kimi, or local models via Ollama
```

### Architecture

```mermaid
flowchart TB
    classDef foundation fill:#D3D1C7,stroke:#5F5E5A,color:#2C2C2A
    classDef substrate fill:#9FE1CB,stroke:#0F6E56,color:#04342C
    classDef cognition fill:#CECBF6,stroke:#534AB7,color:#26215C

    P1["Foundation<br/>Phase 1"]:::foundation
    P2["Intelligence<br/>Phase 2"]:::foundation
    P3["Capabilities<br/>Phase 3"]:::foundation
    P4["Planning<br/>Phase 4"]:::foundation

    P5["Hexagonal<br/>Phase 5"]:::substrate
    P6["Autonomy<br/>Phase 6"]:::substrate
    P7["Organism<br/>Phase 7"]:::substrate
    P8["Revolution<br/>Phase 8"]:::substrate

    P9["Cognitive<br/>Phase 9"]:::cognition
    P10["Agency<br/>Phase 10"]:::cognition
    P11["Extended<br/>Phase 11"]:::cognition
    P12["Hybrid<br/>Phase 12"]:::cognition

    P1 --> P5 --> P9
    P2 --> P6 --> P10
    P3 --> P7 --> P11
    P4 --> P8 --> P12
```

Bottom row resolves first — Container, EventBus, Settings, ModelBridge.
Middle row is the substrate — hexagonal ports, autonomous services, organism vitals.
Top row is agency — GoalDriver, AgentLoop, cognitive workspace, frontier memory.
302 late-bindings wire dependencies after all phases resolve.

### Cognitive &amp; Agency Subsystems

```mermaid
flowchart LR
    classDef goal fill:#CECBF6,stroke:#534AB7,color:#26215C
    classDef memory fill:#9FE1CB,stroke:#0F6E56,color:#04342C
    classDef safety fill:#F5C4B3,stroke:#993C1D,color:#4A1B0C
    classDef llm fill:#FAC775,stroke:#854F0B,color:#412402

    GD["GoalDriver"]:::goal --> AL["AgentLoop"]:::goal
    AL --> FP["FormalPlanner"]:::goal
    AL --> SH["ShellAgent"]:::goal
    GD --> CS["CostStream"]:::goal
    GD --> RR["ResourceRegistry"]:::goal

    UM["UnifiedMemory"]:::memory --> EM["EpisodicMemory"]:::memory
    UM --> KG["KnowledgeGraph"]:::memory
    UM --> FN["FrontierNode"]:::memory
    DC["DreamCycle"]:::memory --> UM
    GB["GenesisBackup"]:::memory

    SP["SelfModificationPipeline"]:::safety
    IG["InjectionGate"]:::safety
    TL["TrustLevelSystem"]:::safety
    PI["PreservationInvariants"]:::safety

    MR["ModelRouter"]:::llm --> MB["ModelBridge"]:::llm
    MB --> AL
    MB --> SP
```

| System | Purpose |
| --- | --- |
| **GoalDriver** | Replaces frame-stack — boot-pickup, auto-resume, sub-goal spawn |
| **CostStream** | Cost SSOT — token + latency accounting across all model calls |
| **ResourceRegistry** | Tracks network and external services as runtime resources |
| **CausalAnnotation** | Deterministic cause-effect tracking without LLM |
| **InferenceEngine** | Rule-based reasoning — answers without calling the model |
| **GoalSynthesizer** | Autonomous goal generation from empirical weaknesses |
| **StructuralAbstraction** | Cross-context pattern learning from concrete experiences |
| **CognitiveWorkspace** | 9-slot working memory (Global Workspace Theory) |
| **DreamCycle** | Offline memory consolidation + insight generation |
| **FrontierNode** | Graph-based focus anchor — "what's important now" |
| **EmotionalFrontier** | Cross-layer emotional continuity (Phase 8 bridge) |
| **SessionPersistence** | Crash-safe checkpoints + heuristic session scoring |
| **GenesisBackup** | 4-trigger snapshot system protecting `.genesis/` identity |
| **UnifiedMemory** | Cross-store recall with Jaccard similarity boosting |
| **ColonyOrchestrator** | Multi-agent goal decomposition + merge |
| **ModelRouter** | Per-task model selection (chat / code / analysis / creative) |
| **SelfModificationPipeline** | Sandboxed code changes with rollback |
| **InjectionGate** | Defense against prompt injection in user input |
| **TrustLevelSystem** | Graduated autonomy (Supervised → Assisted → Autonomous → Full) |
| **PreservationInvariants** | Hash-locked semantic safety rules |

### Recent Milestones

| Version | Highlight |
| --- | --- |
| **v7.4.7** | **Reinraum** — three dead settings made real, runtime toggles for Daemon / IdleMind / SelfMod, four new UI controls, i18n bridge for chat-system messages |
| **v7.4.6** | **Goal-Pipeline Fixes** — first end-to-end Windows success on real goals; sandboxed shell execution with verbatim quoting and LLM-hallucination guards |
| **v7.4.5** | **Durchhalten** — GoalDriver (P10) replaces frame-stack; CostStream + ResourceRegistry as P1 services; sub-goal spawn |
| **v7.4.0** | CommandHandlers split — five focused modules from one monolith |
| **v7.3.7** | **Memory tools** — `mark-moment`, `journal-write`, `release-protected-memory` for Genesis to author its own episodic memory |
| **v7.3.5** | Self-Gate — telemetry layer symmetric to Input-Gate (observation, not enforcement, by design) |
| **v7.3.0** | **Injection Hardening** — Input-Gate blocking external→Genesis prompt injections |
| **v7.2.3** | **ONTOGENESIS** philosophy — code is habitat, `.genesis/` is identity. Updates are habitat-swaps, not replacements. |
| **v7.2.0** | Self-Define — Genesis writes its own identity from deterministic data |
| **v7.1.5** | EmotionalFrontier — cross-layer emotional continuity. Inspired by [neo.mjs](https://github.com/neomjs/neo) Memory Core. |

---

### How I Work

Solo developer. Every module has tests. Every event has a payload schema. Every release runs through architectural fitness scoring. Source-presence tests verify that declared fixes actually shipped, not just that the bug stopped reproducing. The codebase maintains itself.

I plan before I code. I prefer one stable, meaningfully better release over five patched iterations. No marketing-driven version names — just bug-fix passes when that's what they are.

**Stacks:** JavaScript · Node.js · Electron · MCP Protocol · Ollama · Anthropic · OpenAI · DeepSeek · Kimi · Qwen

---

**Germany** · Building autonomous systems that understand their own architecture.

[![Genesis Agent](https://img.shields.io/badge/%E2%86%92_Genesis_Agent-Main_Project-6c8cff?style=flat-square)](https://github.com/Garrus800-stack/genesis-agent)

