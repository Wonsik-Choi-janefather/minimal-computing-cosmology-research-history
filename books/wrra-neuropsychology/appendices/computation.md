# 부록 D 계산 결과와 재현 코드

가상 모형을 Python 표준 라이브러리만으로 실행했다. 외부 자료와 외부 난수는 사용하지 않는다. 다음 값은 사람에게서 관측한 수치가 아니며 단위 없는 모형 값이다.

## D1 기억 흔적 유지

| 갱신 횟수 | 흔적 값 |
| --- | --- |
| 0 | 1.000000 |
| 1 | 0.850000 |
| 3 | 0.614125 |
| 5 | 0.443705 |
| 10 | 0.196874 |

## D2 실패 잔여와 도전 확률

| 실패 횟수 | 잔여 | 자원 1.0 | 자원 0.3 |
| --- | --- | --- | --- |
| 0 | 0.000000 | 0.890903 | 0.813057 |
| 1 | 0.400000 | 0.840238 | 0.736916 |
| 2 | 0.720000 | 0.787178 | 0.663292 |
| 3 | 0.976000 | 0.736217 | 0.597822 |
| 4 | 1.180800 | 0.690214 | 0.542676 |
| 5 | 1.344640 | 0.650422 | 0.497724 |

유지율과 반응 계수는 가상 설정이다. 선택 모형의 자원 효과는 양수, 실패 잔여 효과는 음수로 미리 정했으므로 출력 방향 자체는 경험적 발견이 아니다. 자원별 열은 동일한 잔여를 가진 두 조건을 계산한 것이며, 한 사람의 실제 회복 전후 비교가 아니다.

## D3 재현 코드

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
print("mean", statistics.mean(changes))
print("sample_sd", statistics.stdev(changes))
print("mean_se", statistics.stdev(changes) / math.sqrt(len(changes)))
print("retention_0.95_at_10", 0.95 ** 10)
print("fixed_point", 0.4 / (1 - 0.8))
print("fixed_high", probability(2.0, 1.0))
print("fixed_low", probability(2.0, 0.3))
r = 0.0
for _ in range(5):
    r = 0.8 * r + 0.4
for _ in range(5):
    r = 0.8 * r
print("after_no_new_failure_5", r, probability(r, 1.0))

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
print("scale_change_max_difference", max_difference)
```
판정은 가상 규칙의 실행과 수치 재현이다. 원시 가정에서 자연의 상수를 유도한 결과나 임상 효과의 검증으로 분류하지 않는다. 제시한 코드를 같은 입력으로 실행하면 반올림한 표의 값이 재현되어야 한다.

## D4 학습용 변화량 통계

| 가상 참여자 | 변화량 |
| --- | --- |
| 1 | 4 |
| 2 | 2 |
| 3 | 6 |
| 4 | 2 |
| 5 | 6 |

다섯 독립 변화량의 평균은 4점, 표본 표준편차는 2점, 평균의 표준오차는 0.894427점이다. 실제 참여자의 자료가 아니라 통계량의 구분을 설명하기 위한 가상 입력이다.

## D5 민감도와 식별성 계산

| 조건 | 산출값 |
| --- | --- |
| 유지율 0.95의 10회 뒤 흔적 | 0.598737 |
| 실패 잔여의 고정점 | 2.000000 |
| 고정점에서 자원 1.0의 도전 확률 | 0.475021 |
| 고정점에서 자원 0.3의 도전 확률 | 0.325195 |
| 5회 실패 뒤 새 실패 없이 5회 갱신한 잔여 | 0.440612 |
| 잔여 척도 2배와 계수 절반의 최대 확률 차이 | 0.000000 |

유지율 비교는 가상 규칙의 민감도, 고정점은 해당 갱신식의 성질, 척도 변경의 일치는 잠재 변수의 식별성 문제를 보여 준다. 확장된 재현 코드로 모든 수치를 확인할 수 있다.
