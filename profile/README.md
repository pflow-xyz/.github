## pflow — Petri Net Tools for Verifiable Systems

**Design, simulate, and deploy state machines with explicit causal structure.**

Unlike statistical ML models, Petri nets provide **transparent, deterministic logic** — the model itself is the explanation.

---

### 🎮 Try It Live

Interactive tutorials at **[pilot.pflow.xyz](https://pilot.pflow.xyz)**:

| Demo | What You'll Learn |
|------|-------------------|
| [Tic-Tac-Toe](https://pilot.pflow.xyz/tic-tac-toe/) | Places, transitions, arcs, ODE strategic analysis |
| [ZK Tic-Tac-Toe](https://pilot.pflow.xyz/zk-tic-tac-toe/) | Zero-knowledge proofs with gnark circuits |
| [Coffee Shop](https://pilot.pflow.xyz/coffeeshop/) | Capacity limits, weighted arcs, resource flow |
| [Texas Hold'em](https://pilot.pflow.xyz/texas-holdem/) | Role-based access, guards, event sourcing |
| [Knapsack](https://pilot.pflow.xyz/knapsack/) | Optimization via mass-action kinetics |

---

### 🛠 Projects

| Repository | Description |
|------------|-------------|
| **[pflow-xyz](https://github.com/pflow-xyz/pflow-xyz)** | Browser-based visual editor & ODE simulator |
| **[go-pflow](https://github.com/pflow-xyz/go-pflow)** | Go library — modeling, simulation, code generation |
| **[petri-pilot](https://github.com/pflow-xyz/petri-pilot)** | MCP server for AI-assisted design + full-stack app generation |

```
 pflow-xyz          go-pflow           petri-pilot
 ─────────          ────────           ───────────
 Visual Editor  →   Go Library    →    MCP Server
 ODE Simulator      ODE Solver         Code Generation
 JSON-LD I/O        Smart Contracts    Full-Stack Apps
                         │
                         ▼
              ┌─────────────────────┐
              │  JSON-LD Models     │
              │  pflow.xyz/schema   │
              └─────────────────────┘
```

---

### 🤖 AI-Assisted Development

[petri-pilot](https://github.com/pflow-xyz/petri-pilot) provides **MCP (Model Context Protocol)** tools — AI assistants like Claude can design models and generate complete applications:

```
petri_validate   →  Check model structure
petri_simulate   →  Test state transitions  
petri_analyze    →  Deadlock & liveness analysis
petri_codegen    →  Generate Go backend
petri_frontend   →  Generate ES modules UI
petri_application → Full-stack app from spec
```

---

### 🔗 Links

- **Visual Editor**: [pflow.xyz](https://pflow.xyz)
- **Interactive Demos**: [pilot.pflow.xyz](https://pilot.pflow.xyz)
- **GraphQL Playground**: [pilot.pflow.xyz/graphql/i](https://pilot.pflow.xyz/graphql/i)
- **Blog**: [blog.stackdump.com](https://blog.stackdump.com)
