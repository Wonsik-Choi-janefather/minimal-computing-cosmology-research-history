# Chapter 40 Constructing State Variables and Transformation Rules

### 1 Scene and question

Computing an observed phenomenon requires deciding what to retain as state. Recording every experience enlarges data without automatically improving explanation; discarding necessary traces makes different responses to the same current input difficult to explain. Minimal computation seeks structures satisfying functional criteria between these problems.

Chapter question: How is the minimum state needed for the next update and observation determined?

### 2 Starting points in established research

Starting points for memory, motivation, and measurement connect to the literature in Chapters 15, 21, and 4. The state variables and functions selected here are the author's model design, not equations already estimated by external experiments.

### 3 Validation inputs

The concepts and observational evidence from existing research are identified in this chapter's references and Appendix E. Planned inputs for the WRRA application: candidate states, measurement units, and target outcomes. Measurements and experiments without a separate execution record are research plans, not actual data collected for this manuscript.

### 4 WRRA-specific transformation

Source of the work: the rules, calculations, or validation procedures are the author's WRRA application. Core originates in Choi (2026, W1); the earlier interdisciplinary work is Choi and Choi (2026, W2). Executed values and code are in Appendix D.

Transformation specification: fix updating rules, observation rules, and coefficient sources.

#### 4.1 Specify the question and system boundary first

Adding states without specifying outputs easily complicates a model. Explaining one trial's choice and a day's activity require different inputs and intervals. Internal processing alone or external records and support must also be specified. Minimality is assessed under that goal and boundary.

#### 4.2 States needed for the next update

Different outcomes under identical current input motivate candidate states carrying historical differences. The aim is a small summary preserving necessary distinctions. States producing the same present action are not automatically merged; later conditions may require distinguishing them. Sufficiency must be validated within the specified task and error range.

#### 4.3 Implement updating and observation separately

Separating state change from indicators makes multiple data sources easier to connect. Deterministic updates may have noisy observations, and updates themselves may be stochastic. Combining different uncertainties into one noise term requires stating the simplification's scope. Neural-indicator noise is not equated with intrinsic behavioral-choice probability.

#### 4.4 From existing research to a WRRA application

The examples separate current input, residue, resources, relational coefficients, possible actions, and observation rules. State-updating functions differ from functions reading states as reports or actions. A probability distribution may express several outcomes from one state, but outputting a distribution does not identify every uncertainty source.

### 5 Outputs and execution record

The current output is an explanatory specification of phenomena, variables, and validation paths. Planned output: an executable model specification.

### 6 Falsification conditions and interpretive limits

Falsification condition: restrict interpretations of individual coefficients as real entities if different coefficients generate identical outcomes.

Coefficient sources are marked as measurements, calibration to verified values, or hypothetical settings. Reproducing calibration data is legitimate consistency performance, but does not establish performance elsewhere. Doubling residue scale and halving its output coefficient while retaining outputs can make the two coefficients separately unidentifiable; this is recorded.

#### 6.1 Variable counts and identifiability

Several coefficient combinations may generate one output curve, preventing separate determination. More repetitions under unchanged conditions may not resolve this. Other inputs or observations may be needed. WRRA evaluates both minimum variable count and what the data can distinguish.

#### 6.2 Implementation-check sequence

Match units, check permissible resource and probability ranges, and inspect extreme-condition outputs. Check reproduction under identical inputs before comparing data. These checks concern implementation consistency, not empirical validation. Labeling every coefficient as hypothetical, measured, or calibrated supports later review.

### 7 Current verdict

Current verdict: INFERRED for the WRRA correspondences and explanatory structure; OPEN for empirical fit of the transformation.

Chapter in one sentence: Computational models specify necessary states, updates, and observations and examine alternatives producing identical outputs.

### 8 Next questions and evidence

Next research question: If one state is removed while required function is preserved, do computation and identifiability hold?

Chapter references: W1, W2.
