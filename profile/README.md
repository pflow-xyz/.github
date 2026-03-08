## pflow — Visual Editor for Petri Nets

**One abstraction for state machines, resource flows, game mechanics, and token standards.**

Build models you can simulate, analyze, and generate code from.

**[Open Editor](https://pflow.xyz)** | **[Read the Book](https://book.pflow.xyz)**

---

### Draw → Generate → Prove

| Draw | Generate | Prove |
|------|----------|-------|
| Build state machines visually. Places, transitions, arcs — stored as JSON-LD with content-addressed identity. | AI constrained by the model produces correct code. The topology defines what's valid — the LLM fills in the implementation. | ZK circuits verify every transition without revealing state. Groth16 proofs from net topology. |
| [pflow.xyz](https://pflow.xyz) | [pilot.pflow.xyz](https://pilot.pflow.xyz) | [Read about ZK →](https://blog.stackdump.com/posts/zk-petri-nets) |

Places hold tokens. Transitions move them. Arcs define the rules.
From coffee shops to poker games to blockchain bridges — the same formal structure, the same tools, the same proofs.

---

### Example Models

| Category | Demos |
|----------|-------|
| **Tools** | [Petri Net Viewer](https://pilot.pflow.xyz/pflow), [What is a Petri Net?](https://pilot.pflow.xyz/learn/), [Thinking in Petri Nets](https://pilot.pflow.xyz/patterns/), [ODE Simulation & Prediction](https://pilot.pflow.xyz/advanced/), [Zero-Knowledge Proofs](https://pilot.pflow.xyz/zk-intro/), [Code to Flow](https://pilot.pflow.xyz/code-to-flow/) |
| **Games** | [Tic-Tac-Toe](https://pilot.pflow.xyz/tic-tac-toe/), [ZK Tic-Tac-Toe](https://pilot.pflow.xyz/zk-tic-tac-toe/), [Texas Hold'em](https://pilot.pflow.xyz/texas-holdem/) |
| **Resources** | [Coffee Shop](https://pilot.pflow.xyz/coffeeshop/), [Knapsack](https://pilot.pflow.xyz/knapsack/), [Producer-Consumer](https://pilot.pflow.xyz/producer-consumer/), [Vet Clinic](https://pilot.pflow.xyz/vet-clinic/), [Predator-Prey](https://pilot.pflow.xyz/predator-prey/), [Enzyme Kinetics](https://pilot.pflow.xyz/enzyme-kinetics/) |
| **Workflows** | [Loan Approval](https://pilot.pflow.xyz/loan-approval/), [Hiring Pipeline](https://pilot.pflow.xyz/hiring-pipeline/) |
| **Computation** | [TCP Handshake](https://pilot.pflow.xyz/tcp-handshake/), [Thermostat](https://pilot.pflow.xyz/thermostat/), [Dining Philosophers](https://pilot.pflow.xyz/dining-philosophers/), [Stoplight](https://pilot.pflow.xyz/stoplight/) |
| **Classification** | [Poker Hand](https://pilot.pflow.xyz/poker-hand/) |

---

### Projects

| Repository | Description |
|------------|-------------|
| **[pflow-xyz](https://github.com/pflow-xyz/pflow-xyz)** | Visual editor & ODE simulator — **Draw** |
| **[go-pflow](https://github.com/pflow-xyz/go-pflow)** | Go library — simulation, process mining, ZK proofs, code generation |
| **[petri-pilot](https://github.com/pflow-xyz/petri-pilot)** | MCP server + deterministic full-stack app generation — **Generate** |
| **[book-pflow-xyz](https://github.com/pflow-xyz/book-pflow-xyz)** | "Petri Nets as a Universal Abstraction" — practitioner's guide |

```
Draw (pflow.xyz) ──▶ Generate (go-pflow + petri-pilot) ──▶ Prove (ZK circuits)
      ▲                                                            │
      └────────────────────────────────────────────────────────────┘
```

---

### AI-Assisted Development (MCP)

[petri-pilot](https://github.com/pflow-xyz/petri-pilot) provides **MCP (Model Context Protocol)** tools — AI assistants like Claude can design models and generate complete applications.

**Connect your agent via [Smithery](https://smithery.ai/servers/stackdump/pflow-pilot):**

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

### Links

- **Visual Editor**: [pflow.xyz](https://pflow.xyz)
- **Demos**: [pilot.pflow.xyz](https://pilot.pflow.xyz)
- **Code to Flow**: [pilot.pflow.xyz/code-to-flow](https://pilot.pflow.xyz/code-to-flow/)
- **Book**: [book.pflow.xyz](https://book.pflow.xyz)
- **Blog**: [blog.stackdump.com](https://blog.stackdump.com)
