# Chapter 4 Measurement, Statistics, Reproducibility, and Research Ethics

### 1 Scene and question

Assigning anxiety a number does not measure the whole mind. Questionnaire responses are important data but depend on item meanings, timing, language, and context. Reliability concerns consistency; validity asks whether evidence supports the intended interpretation of a measurement. (Spielman et al., 2020, §7.5 [R1](https://openstax.org/books/psychology-2e/pages/7-5-measures-of-intelligence))

Chapter question: Which observables measure psychological concepts, and how should reproducibility be assessed?

### 2 Starting points in established research

Mean differences should be reported alongside individual differences, effect sizes, and uncertainty. Treating repeated measurements from one person as independent people can inflate evidence. Data used for fitting and evaluation should be separated by appropriate units, such as person or time, to prevent leakage. Replication research examines the conditions under which psychological findings hold. (Lazic, 2010 [R49](https://doi.org/10.1186/1471-2202-11-5); Vabalas et al., 2019 [R50](https://doi.org/10.1371/journal.pone.0224365); Open Science Collaboration, 2015 [R3](https://doi.org/10.1126/science.aac4716))

#### 2.1 Turning psychological concepts into observables

An operational definition specifies how a concept is treated in a particular study. An anxiety score results from particular questions and scoring rules; reaction time is measured between defined starting and ending events. Clear definitions allow other researchers to use the same procedure. No single operational definition exhausts a concept. (Spielman et al., 2020, §2.2 [R1](https://openstax.org/books/psychology-2e/pages/2-2-approaches-to-research))

The measurement record states ownership, time, unit, instrument, error, and missingness. A shorter reaction time may require additional tests to distinguish changes in reading speed, selection time, and hand movement.

#### 2.2 Reliability and validity

Reliability concerns score consistency under specified conditions. Validity concerns support for interpretations and uses of scores. Repeated identical values may fail to measure the intended target. Conversely, when the target changes rapidly, not every change should be interpreted as error. (Spielman et al., 2020, §7.5 [R1](https://openstax.org/books/psychology-2e/pages/7-5-measures-of-intelligence))

A stable-personality test and a same-day fatigue measure have different expectations over time. Item similarity, relationships to other measures, and connections to actual functioning must be assessed for the intended purpose. Applications across languages or populations also require examining whether the same score has the same meaning. (Putnick and Bornstein, 2016 [R44](https://doi.org/10.1016/j.dr.2016.06.004))

#### 2.3 Why means and variation are both needed

If five hypothetical participants change by 4, 2, 6, 2, and 6 points, mean change is 4. Reporting only the mean hides individual variation. The sample standard deviation is 2 points; assuming the five changes are independent, the standard error of the mean is approximately 0.894427 points. These values were directly computed as a learning exercise.

Standard deviation describes dispersion among observations; standard error concerns uncertainty in a specified estimator. A small standard error does not mean everyone responds similarly. Standardized effect sizes can compare outcomes in different units, but the reference variance must be identified. (Altman and Bland, 2005 [R55](https://doi.org/10.1136/bmj.331.7521.903))

#### 2.4 Repeated measurements and information leakage

Five people completing twenty trials each produce one hundred trials but still only five people. Within-person records may share personal characteristics and influences from preceding trials. Analyzing them as one hundred people can underestimate uncertainty in person-level conclusions. Research and analysis units must be specified. (Lazic, 2010 [R49](https://doi.org/10.1186/1471-2202-11-5))

Training and evaluation splits must avoid placing nearly identical records from the same person on both sides when inappropriate to the purpose. Generalizing to new people and predicting the same person's future require different splitting units. Preprocessing and variable selection must also be determined without consulting evaluation data for fair performance assessment. (Vabalas et al., 2019 [R50](https://doi.org/10.1371/journal.pone.0224365))

#### 2.5 What a replication project investigated

The Open Science Collaboration attempted to replicate 100 studies from three psychology journals. It compared several indicators, including effect size and statistical significance, without using one success rate to judge all psychology as true or false. Its contribution was a procedure for measuring published findings again under the same research questions. (Open Science Collaboration, 2015 [R3](https://doi.org/10.1126/science.aac4716))

Scope of evidence: data, procedures, and comparison indicators should be recorded together. Reproducing a WRRA computation and replicating findings in people are separate tests.

### 3 Validation inputs

Research-specification inputs: measurements, sampling, and preprocessing records. The statistical exercise uses the hypothetical independent observations 4, 2, 6, 2, and 6. They are not interpreted as estimates of an effect in actual people.

### 4 WRRA-specific transformation

Transformation specification: estimate variables while including errors and the repeated-measurement structure.

The WRRA measurement ledger specifies variable ownership, units, times, instruments, missing-data treatment, and exclusion criteria. Research collecting memories and emotions includes explanation, consent, withdrawal, and confidentiality as part of its procedures. The hypothetical computations here involve no actual participants. Future human research requires separate review and participant consent.

#### 4.1 Turning psychological concepts into observables — WRRA interpretation

WRRA states and residues follow the same principles. Naming them while postponing measurement makes connection to actual computation difficult.

### 5 Outputs and execution record

Execution record: the hypothetical changes yield a mean of 4 points, sample standard deviation of 2, and standard error of 0.894427. The standard error assumes independent observations. Planned outputs: effect sizes, uncertainty, and replication results. These plans are distinct from the arithmetic exercise.

#### 5.1 Statistical judgments and substantive meaning

A p-value concerns data incompatibility under a specified statistical model; it does not directly state the probability that a hypothesis is true or the effect's size. The American Statistical Association statement emphasizes these distinctions. (Wasserstein and Lazar, 2016 [R23](https://doi.org/10.1080/00031305.2016.1154108)) Interpretation requires considering estimated differences, uncertainty, measurement precision, and practical importance together.

A nonsignificant result alone does not establish equality between conditions. A claim of negligible difference requires a purpose-appropriate equivalence range or sufficient precision. Conversely, large samples can detect very small differences precisely. Their functional or explanatory importance remains a separate judgment.

### 6 Falsification conditions and interpretive limits

Falsification condition: limit the scope if conclusions reverse when measurement method or sample changes.

#### 6.1 A ledger for reproduction and robustness

Reproduction code checks whether the same inputs and settings produce the same results. Replication in different samples and conditions asks a separate question. Robustness checks examine how conclusions change under modest preprocessing changes. These results are not combined into one undifferentiated pass.

The WRRA ledger records data identifiers, coefficient sources, random procedures, program versions, exclusions, and failures. Conditions of breakdown are recorded alongside successful cases. Comparisons with external theories match data, costs, tolerances, and interpretive criteria.

#### 6.2 Designing research that respects participants

People must receive explanations allowing them to understand and choose participation. Collection purposes, procedures, expected burdens, withdrawal, and confidentiality should be clear. The Belmont Report identifies respect, beneficence, and justice as basic principles of human research. (National Commission, 1979 [R24](https://www.hhs.gov/ohrp/regulations-and-policy/belmont-report/read-the-belmont-report/index.html)) These principles do not replace a particular country's legal procedures.

The APA ethics code also addresses consent, deception, debriefing, and related procedures. (APA, n.d. [R25](https://www.apa.org/ethics/code)) Sensitive experiences should not be requested unnecessarily, and data access and retention must be defined. Using past failure or suffering requires examining scientific necessity and burden. Actual research review and consent are separate from executing hypothetical calculations.

#### 6.3 Theoretical strengths and participant rights

WRRA's ownership principle helps document whose experience supplied data as well as who performed calculations. However, the model's technical definition of ownership differs from legal privacy rights. Access to data does not imply permission to use them for every purpose.

Readers should now be able to consider measurement meaning and error, the limits of statistical judgments, and participants' rights together. More precise explanation and protection of human dignity can both be addressed within research design.

### 7 Current verdict

The arithmetic of the hypothetical values is COMPUTATIONAL PASS. It reproduces statistics and comparison quantities, not empirical validation of a WRRA-specific psychological mechanism. Correspondences in the research specification are INFERRED; evaluation using actual data is OPEN.

Chapter in one sentence: Measurement interpretation, statistical uncertainty, and participants' rights belong within the same research procedure.

### 8 Next questions and evidence

Next research question: Do measurement interpretations and effect uncertainty hold when data are split by person?

Chapter references: R1, R3, R22, R23, R24, R25, R44, R49, R50, R55.
