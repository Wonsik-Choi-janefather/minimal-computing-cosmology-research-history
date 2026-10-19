# Appendix D Numerical Results and Reproduction Code

Numerical display rule: ratios, probabilities, and calculated outputs are rounded to six decimal places. Counts, hypothetical input constants, and integer statistics in explanatory prose retain their original notation. Internal calculations are not rounded, and displayed values are not used for subsequent calculations.

These hypothetical models were executed using only Python's standard library, without external data or random numbers. Values are dimensionless model outputs, not human observations.

## D1 Memory-trace retention

| Update count | Trace value |
| --- | --- |
| 0 | 1.000000 |
| 1 | 0.850000 |
| 3 | 0.614125 |
| 5 | 0.443705 |
| 10 | 0.196874 |

## D2 Failure residue and challenge probability

| Failures | Residue | Resources 1.0 | Resources 0.3 |
| --- | --- | --- | --- |
| 0 | 0.000000 | 0.890903 | 0.813057 |
| 1 | 0.400000 | 0.840238 | 0.736916 |
| 2 | 0.720000 | 0.787178 | 0.663292 |
| 3 | 0.976000 | 0.736217 | 0.597822 |
| 4 | 1.180800 | 0.690214 | 0.542676 |
| 5 | 1.344640 | 0.650422 | 0.497724 |

Retention and response coefficients are hypothetical. Resource effects were set positive and failure effects negative, so output direction itself is not an empirical discovery. Columns compare two conditions with identical residue, not one person's observed before–after recovery.

## D3 Reproduction code

```python
import math

# Case 1: hypothetical retention, not measured recall probability
for n in (0, 1, 3, 5, 10):
    trace = 0.85 ** n
    print(n, f"{trace:.6f}")

# Case 2: hypothetical failure residue and challenge probability
def probability(residue, resource):
    score = 1.2 + 0.9 * resource - 1.1 * residue
    return 1.0 / (1.0 + math.exp(-score))

residue = 0.0
for failures in range(6):
    high = probability(residue, 1.0)
    low = probability(residue, 0.3)
    print(failures, f"{residue:.6f}",
          f"{high:.6f}", f"{low:.6f}")
    residue = 0.8 * residue + 0.4

# Additional calculations in the expanded manuscript
import statistics
changes = [4, 2, 6, 2, 6]
print("mean", f"{statistics.mean(changes):.6f}")
print("sample_sd", f"{statistics.stdev(changes):.6f}")
print("mean_se", f"{statistics.stdev(changes) / math.sqrt(len(changes)):.6f}")
print("retention_0.95_at_10", f"{0.95 ** 10:.6f}")
print("fixed_point", f"{0.4 / (1 - 0.8):.6f}")
print("fixed_high", f"{probability(2.0, 1.0):.6f}")
print("fixed_low", f"{probability(2.0, 0.3):.6f}")
r = 0.0
for _ in range(5):
    r = 0.8 * r + 0.4
for _ in range(5):
    r = 0.8 * r
print("after_no_new_failure_5", f"{r:.6f}", f"{probability(r, 1.0):.6f}")

# A rescaled hidden trace can give identical observable probabilities
r1 = r2 = 0.0
max_difference = 0.0
for _ in range(6):
    p1 = probability(r1, 1.0)
    score2 = 1.2 + 0.9 - 0.55 * r2
    p2 = 1.0 / (1.0 + math.exp(-score2))
    max_difference = max(max_difference, abs(p1 - p2))
    r1 = 0.8 * r1 + 0.4
    r2 = 0.8 * r2 + 0.8
print("scale_change_max_difference", f"{max_difference:.6f}")
```

The verdict concerns execution of hypothetical rules and numerical reproduction. It is not derivation of natural constants from primitive assumptions or validation of clinical effects. Reexecuting the code with the same inputs must reproduce the rounded tables.

## D4 Changes for a statistics exercise

| Hypothetical participant | Change |
| --- | --- |
| 1 | 4 |
| 2 | 2 |
| 3 | 6 |
| 4 | 2 |
| 5 | 6 |

The five independent changes have mean 4 points, sample standard deviation 2, and standard error 0.894427. These are hypothetical inputs illustrating distinct statistics, not actual participants' data.

## D5 Sensitivity and identifiability calculations

| Condition | Output |
| --- | --- |
| Trace after 10 updates at retention 0.95 | 0.598737 |
| Fixed point of failure residue | 2.000000 |
| Challenge probability at fixed point, resources 1.0 | 0.475021 |
| Challenge probability at fixed point, resources 0.3 | 0.325195 |
| Residue after 5 failures then 5 updates with no new failure | 0.440612 |
| Maximum probability difference after doubling residue scale and halving its coefficient | 0.000000 |

The retention comparison shows hypothetical-rule sensitivity, the fixed point is a property of the update, and scale equivalence exposes latent identifiability. The extended reproduction code verifies all values.
