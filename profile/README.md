<div align="center">

# SMU-Quantum 🦁

### Quantum algorithms, AI systems, and optimization for hard decision problems

[![GitHub organization](https://img.shields.io/badge/GitHub-SMU--Quantum-181717?logo=github)](https://github.com/SMU-Quantum)
[![Singapore Management University](https://img.shields.io/badge/Institution-SMU-8B1E3F)](https://www.smu.edu.sg)

**Hybrid quantum–classical optimization · Quantum–GenAI co-design · Hardware-aware research**

[Explore repositories](https://github.com/orgs/SMU-Quantum/repositories) · [Research](#research) · [Collaborate](#collaborate)

</div>

---

## About

SMU-Quantum is an open research organization at the [School of Computing and Information Systems](https://computing.smu.edu.sg), **Singapore Management University (SMU)**.

Led by [Prof. Hoong Chuin Lau](https://faculty.smu.edu.sg/profile/lau-hoong-chuin-631), Professor of Computer Science at SMU and Senior Principal Scientist at [A*STAR’s Institute of High Performance Computing](https://www.nqch.sg/researcher/hoong-chuin-lau/), we study how quantum, quantum-inspired, classical, and learning-based methods can work together on difficult decision problems.

Our repositories contain research software, benchmark instances, tutorials, experiment artifacts, and hardware-oriented workflows. The work is grounded in practical constraints: limited qubits, circuit depth, noise, finite shots, penalty design, scalability, and strong classical baselines.

## Research at a glance

<a id="research"></a>

| Research direction | What we study |
| --- | --- |
| **Quantum optimization** | VQE, QAOA, CVaR-VQE, QRAO, PCE, QUBO/Ising mappings, and variational methods for constrained combinatorial problems. |
| **Constraint and penalty design** | Slack-free formulations, custom nonlinear penalties, finite-sampling objectives, CVaR-assisted optimization, feasibility-preserving encodings, and augmented Lagrangian methods. |
| **Learning-augmented optimization** | Reinforcement learning for penalty control, graph shrinking, decomposition, repair, multiplier updates, and adaptive solver policies. |
| **Quantum reinforcement learning** | Equivariant quantum circuits, size-invariant policies, cross-size transfer, TSP/QRL evaluation, and the limits imposed by simulation, finite shots, and hardware noise. |
| **Quantum–GenAI co-design** | LLM-guided closed-loop experimentation that searches over solver families, ansätze, optimizers, sampling budgets, compression strategies, and execution policies. |
| **Noise mitigation and hardware execution** | Light-cone cancellation, hardware-aware backend selection, circuit-resource analysis, fidelity diagnostics, and real-device benchmarking. |
| **Use-inspired operations research** | Vehicle routing, procurement, inventory, supply-chain resilience, maritime networks, finance, and resource planning. |

### Our research principle

Near-term quantum computing is not only an algorithm-design problem. It is also a problem of **representation, decomposition, learning, execution, and measurement**.

We ask when a quantum component is useful, how to make it resource-aware, and how to evaluate it honestly against capable classical alternatives. We do not treat the use of a quantum circuit as evidence of quantum advantage.

## Start here

| If you want to… | Start with… |
| --- | --- |
| Learn quantum optimization | [Quantum Optimization Algorithms](https://github.com/SMU-Quantum/quantum-optimization-algorithms) |
| Run benchmark experiments | [Quantum Optimization Benchmarks](https://github.com/SMU-Quantum/quantum-optimization-benchmarks) |
| Explore adaptive quantum–classical control | [AutoQResearch](https://github.com/SMU-Quantum/autoqresearch) |
| Study vehicle-routing workflows | [Adaptive Quantum CVRP](https://github.com/SMU-Quantum/adaptive_quantum_cvrp) |
| Investigate qubit-efficient encodings | [Pauli Correlation Encoding](https://github.com/SMU-Quantum/pauli-correlation-encoding) |
| Study slack-free constraints | [Cutting Slack](https://github.com/SMU-Quantum/cutting_slack) |
| Browse the full publication record | [Prof. Lau’s SMU profile](https://faculty.smu.edu.sg/profile/lau-hoong-chuin-631) |

## Research

### Recent research highlights

#### Quantum optimization, learning, and hardware

- **[From Circuits to Hardware: Benchmarking Standard and Qubit-Efficient Quantum Optimization on Real Hardware](https://arxiv.org/abs/2607.11637)** — accepted in *Quantum Science and Technology*. Benchmarks VQE, CVaR-VQE, QAOA variants, PCE, and QRAO across MDKP, MIS, QAP, and MSP on IBM Heron processors, covering 247 method–instance combinations. ([DOI](https://doi.org/10.1088/2058-9565/ae94a4) · [Code and artifacts](https://github.com/SMU-Quantum/quantum-optimization-benchmarks/tree/from-circuits-to-hardware))

- **[CVaR-Assisted Custom Penalty Function for Constrained Optimization](https://arxiv.org/abs/2604.20088)** — combines slack-free nonlinear penalties, finite sampling, and CVaR optimization for constrained binary problems, with experiments on Quantinuum H2 hardware.

- **[Light Cone Cancellation for Variational Quantum Eigensolver in Solving Noisy Max-Cut](https://doi.org/10.1038/s41598-025-31798-1)** — published in *Scientific Reports*. Develops a light-cone cancellation framework for reducing noise effects in VQE-based Max-Cut experiments.

- **[AutoQResearch: LLM-Guided Closed-Loop Policy Search for Adaptive Variational Quantum Optimization](https://arxiv.org/abs/2604.24283)** — accepted as a QCE26 Quantum–GenAI Co-Design & Co-Discovery technical paper. Searches adaptive solver-control policies for MIS and CVRP instead of selecting one static solver configuration. ([Repository](https://github.com/SMU-Quantum/autoqresearch))

- **[Qubit-Scalable CVRP via Lagrangian Knapsack Decomposition and Noise-Aware Quantum Execution](https://arxiv.org/abs/2604.22194)** — decomposes CVRP into bounded-width per-vehicle knapsack subproblems, learns multiplier updates, and treats backend and circuit selection as part of the optimization loop. The paper explicitly does not claim quantum advantage.

- **[Learning-Based Graph Shrinking for Quantum Optimization of Constrained Combinatorial Problems](https://doi.org/10.1007/978-3-032-17625-7_3)** — in *Quantum Computing and Artificial Intelligence: QC+AI 2026* (Springer CCIS 2872). Uses reinforcement learning and graph neural networks to guide graph shrinking before quantum solving. ([SMU research record](https://ink.library.smu.edu.sg/sis_research/11034/))

- **[Understanding the Nature of Depth-1 Equivariant Quantum Circuit](https://arxiv.org/abs/2511.10756)** — introduces Size-Invariant Grid Search for analyzing and scaling depth-1 equivariant quantum reinforcement-learning circuits for TSP.

- **[Diagnosing Simulation and Hardware Barriers to Cross-Size Transfer in Equivariant Quantum Reinforcement Learning](https://arxiv.org/abs/2510.14533)** — evaluates cross-size policy transfer across statevector simulation, tensor-network simulation, noisy execution, and hardware, while documenting the limits of scaling claims.

#### Applied optimization and decision intelligence

- **[Securing the Flow: Maritime Energy Resilience under Correlated and Decision-Dependent Disruptions](https://arxiv.org/abs/2605.11990)** — develops a stochastic multi-commodity flow model with decision-dependent disruption probabilities, mean-CVaR risk, and Benders decomposition for maritime energy resilience.

- **[Hybrid Learning and Optimization Methods for Solving the Capacitated Vehicle Routing Problem](https://arxiv.org/abs/2509.15262)** — combines Soft Actor-Critic reinforcement learning with augmented Lagrangian optimization for adaptive penalty control. ([Code](https://github.com/SMU-Quantum/adaptive_quantum_cvrp) · [Springer chapter](https://doi.org/10.1007/978-3-032-17625-7_2))

- **[Cutting Slack: Quantum Optimization with Slack-Free Methods for Combinatorial Benchmarks](https://arxiv.org/abs/2507.12159)** — studies dual ascent, bundle methods, cutting planes, and augmented Lagrangian formulations for TSP, MDKP, and MIS. ([Code](https://github.com/SMU-Quantum/cutting_slack))

- **[Adaptive Graph Shrinking for Quantum Optimization of Constrained Combinatorial Problems](https://arxiv.org/abs/2506.14250)** — introduces constraint-aware shrinking, verification and repair, and adaptive correlation updates for hardware-limited optimization.

- **[A Comparative Study of Quantum Optimization Techniques for Solving Combinatorial Optimization Benchmark Problems](https://arxiv.org/abs/2503.12121)** — compares VQE, CVaR-VQE, QAOA variants, PCE, and QRAO across MDKP, MIS, QAP, and MSP. ([Algorithms](https://github.com/SMU-Quantum/quantum-optimization-algorithms) · [Benchmarks](https://github.com/SMU-Quantum/quantum-optimization-benchmarks))

#### Additional SMU-affiliated quantum-computing papers

The papers below include Prof. Lau and coauthors affiliated with SMU’s School of Computing and Information Systems:

- **[Solving Constrained Combinatorial Optimization Problems with Variational Quantum Imaginary Time Evolution](https://arxiv.org/abs/2504.12607)** — applies VarQITE to the Multiple Knapsack Problem and compares it with QAOA-based approaches.
- **[Implementing Slack-Free Custom Penalty Function for QUBO on Gate-Based Quantum Computers](https://arxiv.org/abs/2504.12611)** — evaluates custom penalty functions that avoid additional slack qubits for constrained binary optimization.
- **[A Feasibility-Preserved Quantum Approximate Solver for the Capacitated Vehicle Routing Problem](https://doi.org/10.1007/s11128-024-04497-5)** — uses a feasibility-preserving encoding and Quantum Alternating Operator Ansatz for CVRP. ([arXiv](https://arxiv.org/abs/2308.08785))

#### Earlier work in procurement and inventory

- **[Quantum Relaxation for Solving Multiple Knapsack Problems](https://arxiv.org/abs/2404.19474)** — combines QRAO-style quantum relaxation with classical linear relaxation for constrained procurement optimization. ([QCE DOI](https://doi.org/10.1109/QCE60285.2024.00086))
- **[Quantum-Enhanced Simulation-Based Optimization for Newsvendor Problems](https://arxiv.org/abs/2403.17389)** — uses quantum amplitude estimation and learned demand distributions for stochastic inventory optimization. ([QCE DOI](https://doi.org/10.1109/QCE60285.2024.00060))
- **[Quantum Monte Carlo Methods for Newsvendor Problem with Multiple Unreliable Suppliers](https://arxiv.org/abs/2409.07183)** — studies risk-aware inventory decisions with quantum Monte Carlo and quantum amplitude estimation.

## Public repositories

The organization currently lists nine public repositories, including the organization profile configuration.

### Core research software and artifacts

| Repository | Focus |
| --- | --- |
| [**autoqresearch**](https://github.com/SMU-Quantum/autoqresearch) | LLM-guided closed-loop policy search, staged confirmation, MIS/CVRP studies, experiment logs, checkpoints, plots, and hardware-run tooling. |
| [**quantum-optimization-benchmarks**](https://github.com/SMU-Quantum/quantum-optimization-benchmarks) | Benchmark instances and evaluation artifacts for quantum optimization, including real-hardware benchmarking. |
| [**quantum-optimization-algorithms**](https://github.com/SMU-Quantum/quantum-optimization-algorithms) | Notebook-based implementations and examples for quantum optimization algorithms. |
| [**adaptive_quantum_cvrp**](https://github.com/SMU-Quantum/adaptive_quantum_cvrp) | Modular CVRP framework combining ALM, SAC reinforcement learning, classical subproblem solving, and Qiskit VQE. |
| [**pauli-correlation-encoding**](https://github.com/SMU-Quantum/pauli-correlation-encoding) | PCE optimization experiments, QUBO-to-Max-Cut transformations, and examples for knapsack, Max-Cut, and MIS. |
| [**cutting_slack**](https://github.com/SMU-Quantum/cutting_slack) | Notebooks and experiments for slack-free and Lagrangian-based constraint handling. |

### Learning and research resources

| Repository | Focus |
| --- | --- |
| [**AMSI_Winter_School_Quantum_Tutorial**](https://github.com/SMU-Quantum/AMSI_Winter_School_Quantum_Tutorial) | Tutorial notebooks introducing quantum optimization. |
| [**nature-of-depth1-eqc**](https://github.com/SMU-Quantum/nature-of-depth1-eqc) | Repository for the depth-1 equivariant quantum circuit study; the repository notes that full code will be released after manuscript acceptance. |
| [**.github**](https://github.com/SMU-Quantum/.github) | Organization-level profile and GitHub configuration. |

## Reproducibility and responsible research

We aim to make research inspectable and extensible through source code, benchmark instances, experiment logs, notebooks, configuration files, and citation metadata where available.

- Research code may be experimental and is not necessarily production-ready.
- Results depend on problem instances, encodings, simulators, hardware, noise, mitigation, and classical baselines.
- A result that uses a quantum algorithm is not, by itself, evidence of quantum advantage.
- Each repository has its own license and reuse requirements. Check its `LICENSE` file before using or redistributing code.
- Please cite the associated paper and repository when building on the work.

## Collaborate

We welcome research collaborations with students, academic groups, quantum-computing teams, and organizations working on difficult decision problems.

- **Research:** propose a benchmark, optimization problem, algorithmic idea, or hardware study.
- **Software:** open an issue with a reproducible example before making a substantial change.
- **Education:** use the tutorial and algorithm repositories as starting points for courses and independent projects.
- **Industry:** discuss logistics, supply-chain, inventory, procurement, finance, maritime, and other resource-planning applications.

For formal research inquiries, contact [Prof. Hoong Chuin Lau](mailto:hclau@smu.edu.sg).

## Quick links

- [SMU-Quantum on GitHub](https://github.com/SMU-Quantum)
- [All public repositories](https://github.com/orgs/SMU-Quantum/repositories)
- [Singapore Management University](https://www.smu.edu.sg)
- [School of Computing and Information Systems](https://computing.smu.edu.sg)
- [Prof. Hoong Chuin Lau — SMU Faculty Directory](https://faculty.smu.edu.sg/profile/lau-hoong-chuin-631)
- [Hoong Chuin Lau — NQCH Researcher Profile](https://www.nqch.sg/researcher/hoong-chuin-lau/)

<div align="center">

<sub>Open research from Singapore Management University · Check each repository for its license and citation instructions.</sub>

</div>
