## pflow — Petri Net Tools for Verifiable Systems

**Design, simulate, and deploy state machines with explicit causal structure.**

Unlike statistical ML models, Petri nets provide **transparent, deterministic logic** — the model itself is the explanation.

---

### Try It Live

**18 interactive demos** at **[pilot.pflow.xyz](https://pilot.pflow.xyz)** — from games to workflows to scientific modeling:

| Category | Demos |
|----------|-------|
| **Games** | [Tic-Tac-Toe](https://pilot.pflow.xyz/tic-tac-toe/), [ZK Tic-Tac-Toe](https://pilot.pflow.xyz/zk-tic-tac-toe/), [Texas Hold'em](https://pilot.pflow.xyz/texas-holdem/), [Poker Hand](https://pilot.pflow.xyz/poker-hand/), [Dining Philosophers](https://pilot.pflow.xyz/dining-philosophers/) |
| **Resources** | [Coffee Shop](https://pilot.pflow.xyz/coffeeshop/), [Producer-Consumer](https://pilot.pflow.xyz/producer-consumer/), [Vet Clinic](https://pilot.pflow.xyz/vet-clinic/) |
| **Workflows** | [Loan Approval](https://pilot.pflow.xyz/loan-approval/), [Hiring Pipeline](https://pilot.pflow.xyz/hiring-pipeline/), [TCP Handshake](https://pilot.pflow.xyz/tcp-handshake/) |
| **Computation** | [Knapsack](https://pilot.pflow.xyz/knapsack/), [Predator-Prey](https://pilot.pflow.xyz/predator-prey/), [Enzyme Kinetics](https://pilot.pflow.xyz/enzyme-kinetics/) |
| **Classification** | [Thermostat](https://pilot.pflow.xyz/thermostat/), [Stoplight](https://pilot.pflow.xyz/stoplight/) |
| **Learning** | [Intro](https://pilot.pflow.xyz/learn/), [Patterns](https://pilot.pflow.xyz/patterns/), [Advanced](https://pilot.pflow.xyz/advanced/), [ZK Intro](https://pilot.pflow.xyz/zk-intro/) |

---

### Projects

| Repository | Description |
|------------|-------------|
| **[pflow-xyz](https://github.com/pflow-xyz/pflow-xyz)** | Browser-based visual editor & ODE simulator |
| **[go-pflow](https://github.com/pflow-xyz/go-pflow)** | Go library — modeling, simulation, process mining, ZK proofs, code generation |
| **[petri-pilot](https://github.com/pflow-xyz/petri-pilot)** | MCP server for AI-assisted design + deterministic full-stack app generation |
| **[pflow-jl](https://github.com/pflow-xyz/pflow-jl)** | Julia framework for Petri net visualization and analysis |

```
 pflow-xyz          go-pflow              petri-pilot
 ─────────          ────────              ───────────
 Visual Editor      Go Library            MCP Server
 ODE Simulator      ODE Solver            Deterministic Codegen
 JSON-LD I/O        Process Mining        Full-Stack Apps
                    ZK Proofs (gnark)
                    Smart Contracts
                          │
              ┌───────────┴───────────┐
              │  JSON-LD Models       │
              │  pflow.xyz/schema     │
              └───────────────────────┘
```

---

### AI-Assisted Development

[petri-pilot](https://github.com/pflow-xyz/petri-pilot) provides **MCP (Model Context Protocol)** tools — AI assistants like Claude can design models and generate complete applications:

```
petri_validate    →  Check model structure
petri_simulate    →  Fire transitions, trace state
petri_analyze     →  Reachability, deadlocks, liveness
petri_codegen     →  Generate Go backend
petri_frontend    →  Generate ES modules UI
petri_application →  Full-stack app from high-level spec
petri_extend      →  Modify existing models
```

The LLM designs models. Templates produce apps. No LLM-generated code in the output.

---

### Key Capabilities

- **Dual execution** — Go backend + JS browser verification produce identical results from identical inputs
- **ODE simulation** — Continuous-time analysis via mass-action kinetics (Tsit5 solver)
- **Zero-knowledge proofs** — Groth16 proofs for state transitions with gnark, Solidity verifier export
- **Process mining** — Alpha/Heuristic miners, rate learning from event logs, predictive monitoring
- **Deterministic codegen** — Event-sourced Go backends, ES module frontends, GraphQL APIs from a single model file
- **Content-addressed storage** — JSON-LD models with IPFS CIDv1 addressing

---

### Links

- **Visual Editor**: [pflow.xyz](https://pflow.xyz)
- **Interactive Demos**: [pilot.pflow.xyz](https://pilot.pflow.xyz)
- **Blog**: [blog.stackdump.com](https://blog.stackdump.com)
