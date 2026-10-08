# Wind Farm Layout Optimisation — SA-GLR

Selected source from a master's dissertation on constrained wind farm layout optimisation. The implementation combines simulated annealing with a geometric layout representation and a binary occupancy encoding. It searches feasible layouts using seven neighbourhood operators and evaluates cost under boundary, obstacle and turbine-spacing constraints.

In the archived experiments, all 50 held-out final layouts passed feasibility checks. Across five WindFLO 2015 scenarios, mean cost was 7.00%–10.75% lower than the supplied genetic-algorithm baseline. Configuration selection used separate seeds from the final held-out evaluation.

This public portfolio copy contains selected SA-GLR algorithm classes and tuning scripts. It deliberately omits the supplied baseline, third-party WindFLO simulator sources, scenario/evaluator classes, vendored JSON libraries, raw scenario datasets, extensive generated results and the submitted dissertation. These excerpts are intended for code review; a full run requires the corresponding simulator, scenario inputs and dependency setup.

Key files: `java/SAGLRAlgorithm.java`, `java/GeometricLayout.java`, `java/GeometricLayoutGenerator.java`, `java/SAGLRResult.java`, and the tuning scripts in `scripts/`.
