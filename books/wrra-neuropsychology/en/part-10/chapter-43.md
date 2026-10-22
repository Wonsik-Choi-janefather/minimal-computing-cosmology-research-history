# Chapter 43 Connecting Neural Activity, Bodily Responses, Experience Reports, and Behavior

### 1 Scene and question

Chapters 41 and 42 computed behavior-related numbers but did not use neural activity as input or output. They therefore do not complete neural implementation. Integration requires putting neural and physiological data into actual computation and explaining measurement timing and error.

Chapter question: How can neural, bodily, and behavioral data on different timescales be connected?

### 2 Starting points in established research

NIMH's RDoC is a framework addressing multiple analytical levels, including molecules, cells, circuits, physiology, behavior, and self-report. (NIMH, n.d. [R7](https://www.nimh.nih.gov/research/research-funded-by-nimh/rdoc/units))

#### 2.1 A study combining state trajectories and intervention

Sauerbrei et al. (2020) examined motor cortex and thalamic inputs during reaching in mice, reporting changes in cortical activity and movement following perturbations and input manipulation. This original study illustrates adding input and intervention evidence to state trajectories in a particular motor system. It does not validate control of human psychology generally or validate WRRA. [[R68](https://doi.org/10.1038/s41586-019-1869-9)]

#### 2.1 A study combining state trajectories and intervention

Sauerbrei et al. (2020) examined motor cortex and thalamic inputs during reaching in mice, reporting changes in cortical activity and movement following perturbations and input manipulation. This original study illustrates adding input and intervention evidence to state trajectories in a particular motor system. It does not validate control of human psychology generally or validate WRRA. [[R68](https://doi.org/10.1038/s41586-019-1869-9)]

### 3 Validation inputs

The concepts and observational evidence from existing research are identified in this chapter's references and Appendix E. Planned inputs for the WRRA application: temporally aligned neural, physiological, behavioral, and self-report data. Measurements and experiments without a separate execution record are research plans, not actual data collected for this manuscript.

#### 3.1 Aligning timescales

Connecting second-scale choices and slower physiological indicators requires specifying when each arises and which interval it reflects. Ignoring delays may change the apparent direction of a connection. Delays selected after seeing outcomes are labeled exploratory. Fixed delays and observation rules must also be checked in other data.

### 4 WRRA-specific transformation

Source of the work: the rules, calculations, or validation procedures are the author's WRRA application. Core originates in Choi (2026, W1); the earlier interdisciplinary work is Choi and Choi (2026, W2). Executed values and code are in Appendix D.

Transformation specification: specify level-specific observation functions and connect them to an updating model.

#### 4.1 Candidate common states and separate observations

Neural activity, physiology, behavior, and experience reports may read a common latent state or different states. Assuming they are copies of one value from the outset obscures disagreements. WRRA specifies which inputs and present states each measurement depends on. Collecting data together differs from connecting mechanisms.

#### 4.2 From existing research to a WRRA application

Even using such data, WRRA must specify its own states, updating rules, and observation paths. Introducing an external framework does not complete implementation inside WRRA.

#### 4.3 Models that read states and models that change them

Successful state-space classification is a result about observation. Control additionally requires specifying how an action or intervention changes UPDATE and how that change passes through the RENDERER into phenotype and measurements. Two models fitting nonintervention records equally well may produce different intervention outcomes if their intervention-dependent update rules differ. This is a logical identifiability example, not a newly executed simulation. [W1, §2.3; R6, [R68](https://doi.org/10.1038/s41586-019-1869-9); suggestion provenance I3]

The WRRA application separately records classification accuracy, next-state computation error, future prediction loss, and error in goal changes following intervention. A failed control model does not automatically invalidate a useful classifier. Conversely, classification accuracy alone does not close a control contract. This distinction already appears in Core 1.0 §2.3; the revision makes it operational for neural-data studies.

### 5 Outputs and execution record

The current output is an explanatory specification of phenomena, variables, and validation paths. Planned outputs: correspondences across data and reproduction across conditions.

### 6 Falsification conditions and interpretive limits

Falsification condition: revise integrated scope and rules if connecting functions fail under other conditions.

#### 6.1 Contributions of additional indicators

Reduced output error after adding a neural indicator counts within its scope, but additional information and evaluation leakage must be checked. More instruments do not always yield a better minimal model. Costs and required distinctions are compared, specifying goals for which extra measurements help.

#### 6.2 Conditions for causal integration

Changing a circuit and examining state and behavior can add pathway evidence. Interventions may affect other components, however, requiring specific designs and comparisons. WRRA records an integrated mechanism only when intervention, internal updating, and observation connections are actually computed. This manuscript contains no neural intervention or analysis of human neural data.

#### 6.3 Verdicts for separate contracts

The present explanatory mapping is INFERRED. The new design has not been fitted to neural data or validated by intervention; its empirical verdict is OPEN. Budgets, observation errors, temporal alignment, and intervention scope must be declared before assigning contract-specific results. Success in interpretation, computation, prediction, or control is not transferred automatically to another contract.

### 7 Current verdict

Current verdict: INFERRED for the WRRA correspondences and explanatory structure; OPEN for empirical fit of the transformation.

Chapter in one sentence: Integrating neural, bodily, and behavioral accounts requires actual internal computation including temporal alignment and observation error.

### 8 Next questions and evidence

Next research question: Do additional physiological indicators improve the distinguishability of a behavior-only model?

A possible study collects choices, heart rate, and neural signals during the same task. After alignment, it compares whether indicators read common or distinct states. Improved explanation after adding an indicator does not prove causality. Manipulation data and independent evaluation should be connected where possible.

Chapter references: R6, R7.
