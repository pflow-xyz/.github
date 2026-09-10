## pflow — One Petri Net, Several Rigorous Lenses

**Declare a net — places, transitions, rates — and simulate it, fit it, and verify it without leaving the same model.**

Arc topology *is* the rate law: a double arc fires quadratically with concentration, a weighted arc scales a flow. Start with ODE — the fastest way to watch a model move — then reach for exact stochastic simulation, parameter fitting, or formal verification against the same declared net.

**[Open Editor](https://pflow.xyz)** | **[Read the Book](https://book.pflow.xyz)**

---

### Model → Simulate → Fit → Verify

| Model | Simulate | Fit | Verify |
|-------|----------|-----|--------|
| Places, transitions, weighted arcs — stored as JSON-LD with content-addressed identity. Arc topology *is* the rate law: a double arc makes a transition fire quadratically with concentration. | Tsit5/RK45 ODE relaxation, exact Gillespie SSA, and chemical-Langevin SDE — three semantics from one declaration. | Gradient-free and gradient-based (forward + adjoint sensitivity) parameter fitting. Every fitted value is still a transition rate. | Reachability, P/T-invariants, and declarative property checking with proved/refuted/unknown verdicts and counterexamples. |
| [pflow.xyz](https://pflow.xyz) | [go-pflow/solver](https://github.com/pflow-xyz/go-pflow/tree/main/solver) | [go-pflow/learn](https://github.com/pflow-xyz/go-pflow/tree/main/learn) | [go-pflow/verify](https://github.com/pflow-xyz/go-pflow/tree/main/verify) |

Same declared model, byte-exact across languages: JS ([pflow.xyz](https://pflow.xyz)), Go ([go-pflow](https://github.com/pflow-xyz/go-pflow)), Rust ([pflow-rs](https://github.com/pflow-xyz/pflow-rs)), and Julia ([pflow-jl](https://github.com/pflow-xyz/pflow-jl), bridged to [AlgebraicPetri.jl](https://github.com/AlgebraicJulia/AlgebraicPetri.jl)).

---

### Start here: ODE Demos

| Demo | What it shows | Link |
|------|----------------|------|
| **Predator-Prey** | Lotka-Volterra dynamics, continuous simulation | [Run](https://pilot.pflow.xyz/predator-prey/) |
| **Enzyme Kinetics** | Michaelis-Menten, biochemical modeling | [Run](https://pilot.pflow.xyz/enzyme-kinetics/) |
| **Knapsack** | Optimization via mass-action kinetics | [Run](https://pilot.pflow.xyz/knapsack/) |
| **ODE Simulation & Prediction** | Walkthrough of the solver itself | [Run](https://pilot.pflow.xyz/advanced/) |

ODE is the fastest way to see a model move, not the whole toolkit — the same declared net also drives exact stochastic simulation, parameter fitting, and formal verification (see the table above). More examples — discrete state machines, workflows, ZK proofs, games — live one level down, in the individual project READMEs below.

---

### Projects

| Repository | Purpose |
|------------|---------|
| **[go-pflow](https://github.com/pflow-xyz/go-pflow)** | Core Go library. ODE/SSA/SDE engines, parameter fitting, reachability & verification. The reference implementation. |
| **[pflow-xyz](https://github.com/pflow-xyz/pflow-xyz)** | Visual editor + browser ODE simulator, held byte-exact to go-pflow. |
| **[pflow-rs](https://github.com/pflow-xyz/pflow-rs)** | Rust port — ODE solvers, token-model DSL, ZK provers. |
| **[pflow-jl](https://github.com/pflow-xyz/pflow-jl)** | Julia port, bridged to AlgebraicPetri.jl for categorical composition and mass-action ODEs. |
| **[petri-pilot](https://github.com/pflow-xyz/petri-pilot)** | MCP server for AI-assisted model design + deterministic app generation from a validated model. |
| **[book-pflow-xyz](https://github.com/pflow-xyz/book-pflow-xyz)** | "Petri Nets as a Universal Abstraction" — practitioner's guide. |

```
Model (pflow.xyz) ──▶ go-pflow (ODE · SSA · SDE · fit · verify) ──▶ pflow-rs / pflow-jl (byte-exact ports)
                                        │
                                        ▼
                              petri-pilot (app generation, MCP)
```

---

### AI-Assisted Model Design (MCP)

[petri-pilot](https://github.com/pflow-xyz/petri-pilot) exposes MCP tools so an agent can design, simulate and verify a model directly:

```
claude mcp add --transport http petri-pilot https://pilot.pflow.xyz/mcp
```

```
petri_validate    →  Check model structure
petri_simulate    →  Fire transitions, trace state (ODE/SSA/SDE)
petri_analyze     →  Reachability, deadlocks, liveness
petri_codegen     →  Generate Go backend
petri_application →  Full-stack app from high-level spec
petri_extend      →  Modify existing models
```

The LLM designs the net. The engines decide what it does. No LLM-generated math in the output.

---

### Links

- **Visual Editor**: [pflow.xyz](https://pflow.xyz)
- **ODE Engine**: [go-pflow](https://github.com/pflow-xyz/go-pflow)
- **Demos**: [pilot.pflow.xyz](https://pilot.pflow.xyz)
- **Book**: [book.pflow.xyz](https://book.pflow.xyz)
- **Blog**: [blog.stackdump.com](https://blog.stackdump.com)
