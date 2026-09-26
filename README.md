# Awesome-Advanced-Planning-n-Scheduling

# Top Advanced Planning & Scheduling (APS) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Production Scheduling, Finite Capacity Planning, Job Shop Optimization, Shop-Floor Sequencing & Manufacturing Resource Planning*  
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Advanced Planning & Scheduling (APS)**. These systems create finite-capacity schedules for manufacturing—sequencing jobs, balancing machines and labor, and reacting to disruptions faster than traditional MRP.

**Examples** include PlanetTogether, Asprova, Siemens Opcenter APS, DELMIA Ortems, Flexis, Preactor, SedApta, Quintiq, Optessa, FLEXSCHE, Oracle Production Scheduling, and Infor APS (the category leaders).

**Open-source emphasis**: Full commercial APS suites dominate discrete and process manufacturing. Open strength lies in **constraint solvers**—**Timefold** (OptaPlanner successor), **OR-Tools**, and job-shop research code—used to build custom schedulers. This section lists every significant relevant project found.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[PlanetTogether](https://www.planettogether.com/)**  
  Popular APS platform for finite capacity scheduling, what-if analysis, and multi-plant production planning.

- **[Siemens Opcenter APS, DELMIA Ortems (Dassault)](https://www.siemens.com/)**  
  Enterprise APS within major MES/MOM suites—detailed scheduling integrated with shop-floor execution.

- **[Asprova, FLEXSCHE, Preactor (Siemens legacy), SedApta](https://www.asprova.com/)**  
  Specialized APS products strong in discrete manufacturing, high-mix scheduling, and rapid rescheduling.

- **[Quintiq (Dassault), Optessa, Flexis](https://www.3ds.com/)**  
  Advanced planning and optimization platforms for complex supply chain and production scheduling problems.

- **[Oracle Production Scheduling, Infor APS](https://www.oracle.com/)**  
  APS modules within broad ERP/supply-chain suites for enterprise manufacturers.

- **[Other commercial APS platforms](https://www.planettogether.com/)**  
  Additional solutions for process industries, batch scheduling, and cloud APS.

## Open-Source GitHub Projects

- **[Timefold Solver](https://github.com/TimefoldAI/timefold-solver)**  
  Leading open-source (Apache 2.0) constraint solver for Java/Kotlin—job shop scheduling, task assignment, maintenance scheduling, rostering; continuation of OptaPlanner by its original team.

- **[Google OR-Tools](https://github.com/google/or-tools)**  
  Open suite of optimization tools—CP-SAT, routing, linear/integer programming—widely used to build custom production and job-shop schedulers.

- **[OptaPlanner (legacy) & OptaPy](https://github.com/kiegroup/optaplanner)**  
  Historic open constraint solver (now largely superseded by Timefold) and Python bindings still referenced in existing deployments.

- **[Job shop scheduling research implementations](https://github.com/search?q=job+shop+scheduling+OR+JSSP+open+source)**  
  Academic and community solvers for classic job-shop and flow-shop problems used as building blocks.

- **[OptaWeb / scheduling UI quickstarts](https://github.com/TimefoldAI/timefold-quickstarts)**  
  Open quickstarts for employee rostering, maintenance, and job-shop-style problems on Timefold.

- **[PuLP, Pyomo & Python modeling stacks](https://github.com/coin-or/pulp)**  
  Open modeling languages for linear and mixed-integer programs that encode APS-style constraints.

- **[Discrete-event simulation open tools](https://github.com/search?q=manufacturing+simulation+OR+shop+floor+simulation+open+source)**  
  Simulation frameworks used to validate schedules before release to the shop floor.

- **[ERPNext manufacturing + custom schedulers](https://github.com/frappe/erpnext)**  
  Open ERP with manufacturing modules that teams extend with Timefold/OR-Tools for finite scheduling.

### Additional Strong Open-Source Options

- **Constraint AI solver**: Timefold for production-grade scheduling models in Java/Kotlin.
- **General optimization**: OR-Tools CP-SAT for flexible custom APS engines.
- **Python stacks**: PuLP/Pyomo + heuristics for lighter or research schedulers.
- **Composable stacks**: ERP/MES orders → Timefold/OR-Tools → Gantt/dispatch UI.
- Commercial APS still leads in out-of-the-box shop calendars, BOM/routing integration, and industry templates.

**Frameworks for building custom systems**:  
**Timefold Solver** and **Google OR-Tools** are the strongest open foundations for APS-style optimization.  
Model jobs, machines, tools, and calendars as constraints; expose results via Gantt or MES interfaces.  
Commercial APS (PlanetTogether, Siemens Opcenter, Asprova, DELMIA Ortems, Quintiq, etc.) deliver complete manufacturing scheduling products.  
Advanced manufacturers sometimes embed open solvers inside custom systems; most plants adopt commercial APS for speed and support. Fully open APS is achievable for specialized problem types with in-house optimization expertise.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Production schedules affect safety, quality, and delivery commitments. Validate any scheduler against real constraints (maintenance, skills, tooling, material) before shop-floor use. Incorrect schedules can cause costly downtime or missed orders.
- Open-source solvers offer full control but require modeling expertise and integration work. Commercial APS platforms shift product depth and support to the vendor. Neither replaces accurate master data and disciplined production execution.

---

**Made for manufacturing engineers, supply chain planners, and teams optimizing the shop floor.**  
Let's expand open planning solvers while recognizing the industry depth and integration that leading commercial APS platforms deliver.
