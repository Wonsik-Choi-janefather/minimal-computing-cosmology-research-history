# Chapter 41 Computational Example One: Maintaining a Memory Trace

### 1 Scene and question

Consider a name learned yesterday that does not immediately come to mind today. Before explaining all memory, we first compute a rule maintaining one trace without new input. The following is a hypothetical example addressing that question alone.

Chapter question: Which trace values does a fixed maintenance rule actually produce?

### 2 Starting points in established research

Chapter 15 distinguishes encoding, retention, and retrieval; Chapter 16 addresses alternative explanations of forgetting. This example preserves those distinctions while computing one maintenance rule.

### 3 Validation inputs

Execution inputs: hypothetical initial value 1, retention rate 0.85, and update counts. These are hypothetical settings, not human measurements or constants calibrated from the literature. Values and code are provided here and in Appendix D.

### 4 WRRA-specific transformation

Source of the work: the rules, calculations, or validation procedures are the author's WRRA application. Core originates in Choi (2026, W1); the earlier interdisciplinary work is Choi and Choi (2026, W2). Executed values and code are in Appendix D.

Transformation specification: multiply the preceding trace by the retention rate to compute the next trace.

The smallest example maintains one trace at a fixed proportion per update. Starting at 1, each next value is 0.85 times the previous value while there is no new input. These are hypothetical settings rather than measured or calibrated constants. An update has not been mapped to actual seconds or days.

#### 4.1 Complete input and rule specification

Inputs are initial trace 1, retention ratio 0.85, and specified update counts. New input is zero at every step. The model therefore concerns dimensionless trace maintenance, not new learning or retrieval success. Real time and neural implementation remain unmapped.

#### 4.2 What cannot be known without an observation rule

The model gives no grounds for equating a halved trace with halved recall probability. Cues and testing methods can yield different outcomes from the same trace. Recall rates require a separate trace-to-observation function. This preserves the distinction between numerical execution and reproduction of memory phenomena.

### 5 Outputs and execution record

Execution record: fixed inputs and Appendix D code computed trace values and sensitivity to retention rate. These are actually executed hypothetical-model outputs, distinct from empirical observations.

The results are 1.000000 after 0 updates, 0.850000 after 1, 0.614125 after 3, 0.443705 after 5, and 0.196874 after 10. The structure implements different remaining traces as update counts change despite equal initial input. Trace values are not recall probabilities; retrieval cues and observation rules must be added to compute those.

#### 5.1 Changing the retention rate

Holding other conditions fixed and changing retention to 0.95 yields 0.598737 after 10 updates, versus 0.196874 at 0.85. This directly demonstrates rule sensitivity, not the discovery of two kinds of people. Empirical comparison requires calibration from human data and specified observation rules.

### 6 Falsification conditions and interpretive limits

Falsification condition: numerical errors are implementation failures; mismatch with actual data requires revision of the maintenance model.

#### 6.1 Which data change the model?

If delay-specific data do not fit one rate, intervening experience and interference should be examined. Multiple trace components or condition-dependent rates may be introduced if needed. Before adding variables, specify which difference each term must reproduce. Compare simpler alternatives calibrated to the same data as well as more complex models.

### 7 Current verdict

The achievement is actual numerical execution of a maintenance rule, not reproduction of human forgetting curves. Actual data could calibrate the rate and fix retrieval rules for testing at other delays. If one rate cannot explain repeated measurements, alternatives such as interference or multiple maintenance modes are examined.

#### 7.1 Assessing reproduction performance

Reproducing table values from identical inputs shows consistency between code and rules. Reproducing a known recall curve with a data-calibrated rate could add consistency and explanatory performance. A subsequently fixed model deriving unmeasured-delay outcomes would provide predictions. The present example executes hypothetical settings and sensitivity calculations.

COMPUTATIONAL PASS is restricted to execution and reproduction of the specified hypothetical rules. Empirical fit to human behavior and neural mechanisms is OPEN. Mathematically derived relationships receive EXACT only with assumptions and derivation scope stated; numerical success is not expanded into proof of the whole Core.

Chapter in one sentence: A hypothetical maintenance rule reproduces trace values; connecting them to recall requires additional rules.

### 8 Next questions and evidence

Next research question: Do retention and observation rules fitted to actual memory data work at other delays?

Chapter references: R1.
