# Chapter 42 Computational Example Two: Failure Experience and the Next Choice

### 1 Scene and question

Consider the hypothetical choice of trying again after five failures at the same task. Separating remaining effects of failure from currently available resources allows condition-specific choices to be computed for the same history.

Chapter question: Which choice probabilities does a fixed model connecting failure residue and current resources produce?

### 2 Starting points in established research

Chapter 13 distinguishes learning and behavioral consequences; Chapter 21 addresses motivation and costs; Chapter 24 addresses resource conditions. Coefficients here are hypothetical, not estimated in those studies.

### 3 Validation inputs

Execution inputs: a hypothetical failure sequence and resource values 1.0 and 0.3. These are hypothetical settings, not human measurements or constants calibrated from the literature. Values and code are provided here and in Appendix D.

### 4 WRRA-specific transformation

Source of the work: the rules, calculations, or validation procedures are the author's WRRA application. Core originates in Choi (2026, W1); the earlier interdisciplinary work is Choi and Choi (2026, W2). Executed values and code are in Appendix D.

Transformation specification: connect failure-residue updating and resource conditions to choice probabilities.

Initial residue is 0, each failure adds 0.4, and the previous residue retains a proportion of 0.8. Challenge probability applies a logistic function to a score consisting of baseline 1.2 plus 0.9 times resources minus 1.1 times residue. Every coefficient is hypothetical; action-availability conditions are assumed equal.

#### 4.1 Failure inputs and action boundaries

Failure counts are externally supplied. Feedback through which chosen actions change later failure probabilities is not implemented. Resources 1.0 and 0.3 are hypothetical conditions without one-to-one correspondence to measured fatigue. Available actions are held constant while challenge-choice probability varies.

### 5 Outputs and execution record

Execution record: Appendix D's inputs and code computed choice probabilities by failure count and resource condition. Fixed points, cessation of new failures, and latent-scale changes were also checked. The values below are actual executions of the hypothetical model.

Before failure, challenge probabilities are 0.890903 for resources 1.0 and 0.813057 for 0.3. After five failures, residue is 1.344640 and probabilities are 0.650422 and 0.497724. Thus present resources alter outputs under identical experiential residue.

#### 5.1 Conditional limit under continuing failure

With identical failures continuing, the update's fixed point is residue 2: 0.8 times 2 plus 0.4 equals 2. At that state, probabilities are 0.475021 for resources 1.0 and 0.325195 for 0.3. This is a mathematical property of the specified rule, not a universal final value of actual behavior.

#### 5.2 Stopping new failure input

After five failures, five maintenance-only updates yield residue 0.440612 and challenge probability 0.834150 at resources 1.0. This implements decay under zero new input, not successful experience. It is not an actual treatment or recovery effect, and the time unit remains unspecified.

### 6 Falsification conditions and interpretive limits

Falsification condition: revise the signs and rules if effects persist in the opposite direction after actual conditions are matched.

#### 6.1 Identical outputs and different internal scales

Doubling residue scale and failure increments while halving the residue coefficient in the output equation gives identical choice probabilities. Choice data alone therefore cannot independently establish residue's absolute magnitude and output sensitivity. Fixing a scale reference or adding observations is necessary. This identifiability issue should be checked before using a model.

### 7 Current verdict

Failure's negative effect follows from the chosen rule, not a finding that everyone reduces challenges after failure. A fixed model must be compared with actual choices to assess direction and magnitude. After calibration, unmeasured-condition outputs count as that fixed model's predictions. The present verdict concerns hypothetical computation.

COMPUTATIONAL PASS is restricted to execution and reproduction of the specified hypothetical rules. Empirical fit to human behavior and neural mechanisms is OPEN. Mathematically derived relationships receive EXACT only with assumptions and derivation scope stated; numerical success is not expanded into proof of the whole Core.

Chapter in one sentence: Probabilities connecting failure residue and resources were computed; fit to human behavior remains future work.

### 8 Next questions and evidence

Next research question: After calibration to actual trials, can choice distributions under new resource conditions be derived?

#### 8.1 Moving to actual data

Data can match current difficulty and reward information while investigating previous-feedback effects. Coefficients are calibrated, fixed, and evaluated using person- or condition-level splits. Opposite effects require revising signs or update rules. Specifying a direction in hypothetical computation must not be reported as an empirical discovery.

Chapter references: R1.
