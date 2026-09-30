# 제3부 현실 렌더러 아키텍처

## 제3부 현실 렌더러 아키텍처

공동 실현에서 Einstein branch까지

## 제3부를 여는 말

제3부는 앞에서 형성된 직관을 WRRA의 최소 명세로 고정하고, 그 명세가 기존 물리학의 언어에서 어떻게 구현될 수 있는지를 살펴본다. 중심에는 2026년 8월 27일 공개된 renderer path independence 논문, 이를 복원가능성·metric faithfulness로 보수한 v1.1, 그리고 반복된 rendering의 시간균일 안정성을 다룬 v1.2가 있다.

이 부의 핵심은 특정 5차원 모형을 우주의 궁극적 실재로 선언하는 것이 아니다. 5차원 parent는 가능한 renderer 가운데 하나이며, Einstein gravity도 명시적인 추가 가정 아래 선택되는 조건부 저에너지 branch다.

WRRA가 살아남으려면 아름다운 해석을 넘어 서로 다른 구현 경로의 관측동등성, anomaly-free constraint closure와 입력하지 않은 자료에 대한 예측을 보여야 한다. 제3부는 현재 닫힌 구조와 다음 검증의 경계를 함께 기록한다.

## 18장 WRRA는 무엇을 설명하려는가

Wonsik Reality-Renderer Architecture, 곧 WRRA는 밑바닥의 어떤 원천이 우리가 관측하는 현실과 그대로 같다고 가정하지 않는다. 원천에는 더 많은 자유도와 연속체, 잠재적 관계가 있을 수 있으며, 관측 가능한 3+1차원 현실은 그것들이 하나의 국소적이고 일관된 형태로 공동 실현된 결과다.

이 관점에서 현실은 원천의 복사본이 아니라 phenotype이다. 생물학에서 같은 유전정보도 발현 과정과 환경에 따라 구체적인 형질로 나타나듯, 물리적 원천도 renderer의 규칙과 경계조건을 통과한 뒤 질량·전하·스핀·위치를 가진 대상으로 나타난다. 비유의 목적은 생물학을 물리학에 억지로 옮기는 것이 아니라 원천과 관측결과 사이의 구현 층을 분리하는 데 있다.

WRRA의 최소 구조는 SOURCE, RENDERER, PHENOTYPE의 세 층이다. SOURCE는 가능한 자유도와 잠재적 상태를 제공하고, RENDERER는 허용관계와 국소성·대칭·전달·기록 조건을 적용하며, PHENOTYPE은 하나의 관측 가능한 물리적 현실로 드러난다.

_P = R(S; RELATION, BOUNDARY, θ)_ (3.1)

RENDERER 안에는 RELATION과 BOUNDARY가 들어간다. RELATION은 무엇이 서로 결합하고 보존될 수 있는지를 정하며, BOUNDARY는 그 결과가 다른 계와 상호작용해 기록 가능한 차이로 남는 인터페이스다. 차원필터와 공통전달자는 renderer의 후보 모듈이지 WRRA 전체와 동일하지 않다.

따라서 WRRA는 ‘우주가 컴퓨터 시뮬레이션이다’라는 존재론을 요구하지 않는다. 외부 컴퓨터나 프로그래머를 가정하지 않고도, 원천의 가능성이 제한된 관측현실로 구현되는 구조를 물을 수 있다. 최소계산은 renderer가 중복을 피하고 공통 관계를 재사용한다는 운영원리다.

현재 WRRA가 동결한 것은 하나의 최종 작용이 아니라 최소 명세다. 물리적 구현 후보는 이 명세를 만족하는지 시험받으며, 특정 5차원 모형이나 Bessel carrier가 실패해도 아키텍처 전체가 자동으로 무너지지 않는다. 반대로 후보 하나가 작동한다고 WRRA 전체가 증명되는 것도 아니다.

_WRRA = {S, R, P; compatibility, locality, recordability}_ (3.2)

### 관련 공개 연구

**Wonsik Reality-Renderer Architecture v1.0** [10.5281/zenodo.22122349](https://doi.org/10.5281/zenodo.22122349)

## 19장 공동 실현된 물리적 대상

전자 하나를 생각해보자. 우리는 전자의 질량을 한 실험에서, 전하를 다른 실험에서, 스핀을 또 다른 실험에서 측정할 수 있다. 하지만 자연 속의 전자는 이 속성들을 서로 무관한 표찰로 따로 소유하지 않는다. 같은 사건과 같은 전파이력 속에서 모든 속성이 공동으로 귀속된다.

WRRA는 이 공동 귀속을 joint phenotype이라 부른다. 물리적 대상은 질량 연산자의 고유값, 게이지 표현, 로런츠 표현, 국소 위치를 단순히 한 줄에 나열한 것이 아니다. 이들이 같은 국소 관측대수와 같은 번역 작용 아래에서 양립하고 지속되어야 한다.

_P\_joint = (m, q, s, x) │ (A\_local, T\_a)_ (3.3)

안정 입자는 실수축의 pole로, 전자 같은 하전입자는 연질광자 구름 때문에 엄밀한 단일입자 pole 대신 infraparticle threshold로 나타날 수 있다. 불안정 입자는 해석적으로 연장된 공명 pole로 기술되며, 양성자 같은 합성체는 gauge-invariant composite state로 실현된다. renderer는 이 서로 다른 spectral ownership을 구별해야 한다.

_stable pole ⊕ infraparticle threshold ⊕ resonance ⊕ composite_ (3.4)

이 구별이 없으면 질량을 생성했다고 말하면서 실제로는 공명폭을 잘못 읽거나, gauge-dependent 장을 물리적 입자와 동일시하거나, 합성체의 질량을 기본장 매개변수처럼 취급하는 오류가 생긴다. WRRA의 장부는 각 관측량이 어느 spectral sector에 속하는지 먼저 묻는다.

공동 실현은 위치 문제도 포함한다. 한 대상의 전하와 질량이 서로 다른 시공간 위치에서 정의된다면 검출 가능한 입자가 되지 못한다. 모든 속성은 같은 번역이력과 국소 상호작용점에서 함께 이동하고 반응해야 한다.

이것이 renderer가 단순한 분류기가 아닌 이유다. 필터는 통과 여부를 정할 수 있지만, renderer는 통과한 자유도들을 하나의 물리적 정체성으로 결속하고 시간에 따라 보존해야 한다.

### 관련 공개 연구

**Wonsik Reality-Renderer Architecture v1.0** [10.5281/zenodo.22122349](https://doi.org/10.5281/zenodo.22122349)

## 20장 가시 인터페이스와 숨은 연속체

WRRA v1.0은 가시 현실과 숨은 원천 사이를 self-adjoint block architecture로 나눈다. 가시 부문은 우리가 입자와 장으로 읽는 인터페이스이고, 숨은 부문은 더 넓은 연속체나 아직 직접 관측되지 않은 자유도를 포함할 수 있다.

전체 Hamiltonian을 가시공간과 숨은공간의 블록으로 나누면, 가시 부문의 유효 동역학은 숨은 부문을 단순히 삭제한 결과가 아니다. resolvent를 통해 숨은 부문이 self-energy와 스펙트럼 밀도로 되돌아온다. 이 구조는 열린 계의 효과를 보존하면서도 전체 연산자의 자기수반성을 유지하는 표준적 길을 제공한다.

_H = \[\[H\_vis, V], \[V†, H\_hid]]_ (3.5)

_G\_vis(z) = \[z − H\_vis − V(z−H\_hid)⁻¹V†]⁻¹_ (3.6)

중요한 점은 숨은 연속체가 곧 암흑물질이나 다른 우주라고 단정되지 않는다는 것이다. 그것은 renderer 구현에서 가시 인터페이스 밖에 있는 자유도의 수학적 소유권이다. 실제 물리적 해석은 pole, threshold, 산란자료와 우주론적 관측을 통해 따로 검증해야 한다.

Bessel common carrier는 이런 숨은 연속체의 한 후보다. 하나의 압축된 스펙트럼 채널이 여러 내부 방향을 공통으로 운반하고, 경계에서 유효한 물질 상태를 내보내는 그림이다. Bessel이라는 이름은 외부 프로그램이 아니라 특정 미분방정식과 그 스펙트럼 구조에서 유래한다.

하지만 exact Bessel transport가 모든 sector에서 그대로 유지된다고 가정하면 안 된다. 스칼라 안정화와 게이지 상호작용, 결함과 경계조건은 스펙트럼을 변형할 수 있다. 따라서 정확한 Bessel core와 변형된 sector, 저에너지 matching 영역을 구별해야 한다.

이 블록 구조의 장점은 실패를 국소화한다는 데 있다. 특정 숨은 연속체의 자외선 거동이 실패하면 그 구현을 폐기할 수 있지만, 원천과 가시 phenotype을 분리해야 한다는 WRRA의 상위 질문까지 함께 버릴 필요는 없다.

### 관련 공개 연구

**Quantum Realization Hierarchy of the Bessel Common Carrier** [10.5281/zenodo.22121400](https://doi.org/10.5281/zenodo.22121400)

## 21장 양자적 실현에는 여러 층이 있다

Bessel common carrier를 양자적으로 실현하는 길은 하나가 아니다. 연구 계보는 세 가지 수준을 구분했다. 첫째는 유한 Jacobi runtime, 둘째는 단일 generalized-field spectral runtime, 셋째는 warped defect-holographic parent다. 〔부록 D ‘야코비 행렬’ 참조〕

_Jacobi runtime → spectral field → warped defect parent_ (3.7)

유한 Jacobi runtime은 연속 스펙트럼을 유한 행렬과 이산 상태로 근사한다. 가장 보수적이고 계산 가능하며 국소적인 양자 runtime이다. pole과 residue, 제한된 에너지 창의 응답을 수치적으로 맞추기 좋지만, 정확한 무한 연속체를 그대로 보존하지는 않는다.

단일 generalized field는 하나의 비국소 또는 pseudodifferential spectral symbol 안에 압축된 연속체를 보존한다. 독립적인 무한 개의 하전장을 도입하지 않고도 목표 two-point function을 나타낼 수 있지만, 상호작용 subgraph의 폐쇄와 gauge completion, renormalization이 별도의 문턱이 된다.

warped defect parent는 한 단계 더 기하학적이다. 더 높은 차원의 국소 장이 경계나 결함에서 Bessel형 스펙트럼을 만든다. bulk causality와 양의 spectral compression의 소유권을 제공할 수 있지만, 이것이 자연의 근본 차원이라는 뜻은 아니다.

세 runtime이 같은 양의 two-point spectral target을 제한된 matching window에서 재현하더라도 물리적으로 동일한 이론은 아니다. 장의 개수, 국소성, gauge completion, 자외선 비용과 unitarity가 정의되는 Hilbert 공간이 다르다.

_G₁(E) ≈ G₂(E) on E∈W ⇏ Theory₁ = Theory₂_ (3.8)

그래서 ‘양자적 실현 단계가 끝났다’는 말도 층별로 해야 한다. two-point 재현, 상호작용 일관성, one-loop 상대폐쇄, all-loop completion, 표준모형 embedding은 서로 다른 문턱이다. 현재 연구는 일부 층을 닫았지만 전체 양자중력을 완성하지는 않았다.

### 관련 공개 연구

**Conditional One-Loop Relative BRST Closure of the Single-Field Bessel Spectral Carrier** [10.5281/zenodo.22121047](https://doi.org/10.5281/zenodo.22121047)

**Quantum Realization Hierarchy of the Bessel Common Carrier** [10.5281/zenodo.22121400](https://doi.org/10.5281/zenodo.22121400)

## 22장 가능한 국소 Standard-Model parent

양자 실현 계보에서 5차원 Einstein–scalar parent는 WRRA의 첫 명시적 국소 구현 chassis로 제시되었다. 유한 warped interval을 scalar boundary condition으로 안정화하고, 그 위에 Bessel radial core와 카이럴 표준모형 zero mode를 배치하는 구조다.

_ds² = e^(−2A(y))η\_μνdx^μdx^ν + dy²_ (3.9)

이 모형의 장점은 길이와 gap, chirality와 전달을 하나의 국소 장이론 틀에서 함께 다룰 수 있다는 점이다. 유한 Kaluza–Klein gap은 저에너지 가시부문과 무거운 모드를 구분하며, generation-universal transport는 관측된 Yukawa·CKM·PMNS 자료를 보존하는 방향으로 구성된다.

그러나 ‘보존한다’와 ‘예측한다’는 다르다. 관측된 Yukawa와 혼합자료를 matching input으로 넣어 저에너지에서 유지하는 것은 구현 가능성의 검사다. 그 수치를 geometry만으로 처음부터 도출한 것은 아니다.

_O\_low(μ) = Match\_μ\[O\_parent; θ\_obs]_ (3.10)

또한 단순한 Kaluza–Klein 절단으로 저에너지 이론을 정의해서는 안 된다. gauge-covariant matching과 threshold 보정이 필요하며, scalar-deformed sector와 exact Bessel sector를 분리해야 한다. 안정성, anomaly inflow, flavor counterterm, BRST와 cutoff corridor 조건도 함께 충족해야 한다.

따라서 5차원 parent의 정확한 지위는 possible local implementation chassis다. WRRA의 최종 본체도 아니고 자연이 반드시 사용하는 구조도 아니며, 모든 스케일에 유효한 근본이론도 아니다.

이 제한은 약점만은 아니다. 가능한 renderer 가운데 하나를 실제 기존 장이론 언어로 구축했다는 것은 아키텍처가 순수한 은유에 머물지 않는다는 뜻이다. 이제 더 깊은 질문은 서로 다른 구현 경로가 같은 관측현실을 내놓으려면 어떤 조건이 필요한가이다.

### 관련 공개 연구

**A Stabilized Local Standard-Model Parent for the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22123134](https://doi.org/10.5281/zenodo.22123134)

## 23장 Renderer path independence

같은 물리적 경계에서 출발해 같은 경계에 도달하는 두 rendering 경로가 있다고 하자. 중간의 slice와 gauge 선택, 분해 순서가 다르더라도 최종 관측내용이 달라지지 않아야 한다. WRRA는 이를 renderer path equivalence 또는 path independence라 부른다.

_R\_γ₁(B\_f,B\_i) ≃\_gauge R\_γ₂(B\_f,B\_i)_ (3.11)

이 원리는 모든 중간 표현이 문자 그대로 같아야 한다는 뜻이 아니다. gauge redundancy에 해당하는 차이는 허용되지만 gauge-invariant observable은 일치해야 한다. 따라서 경로독립성은 관측내용과 표현의 중복을 분리하는 조건이다.

작은 deformation을 서로 다른 순서로 적용했을 때 차이가 다시 허용된 deformation으로 닫혀야 한다. 국소 slice가 비퇴화 시공간기하에 embedding될 수 있다면 hypersurface-deformation algebra가 이러한 변형의 운동학을 제공한다.

정준 표현에서는 이 변형들이 first-class constraint로 나타난다. constraint algebra가 닫히지 않으면 서로 다른 slicing 경로가 서로 다른 물리상태를 만들거나 anomaly를 남긴다. 그러면 renderer는 동일한 현실을 일관되게 구현하지 못한다.

_{H\[N],H\[M]} = D\[qᵃᵇ(N∂\_bM−M∂\_bN)]_ (3.12)

하지만 path independence 자체가 Einstein 방정식을 직접 만들어낸다고 말하면 과장이다. 그것은 필요한 gauge와 deformation 구조를 요구한다. 어떤 동역학 branch가 선택되는지는 사용한 canonical variable, 국소성, 미분차수와 추가 자유도에 달려 있다.

이 원리는 WRRA를 검증 가능한 방향으로 바꾼다. 서로 다른 renderer 경로에서 계산한 boundary observable의 차이를 측정할 수 있고, constraint anomaly나 source-clock leakage가 남는다면 해당 구현은 실패한다.

### 관련 공개 연구

**Renderer Path Independence and the Einstein Branch of the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22124886](https://doi.org/10.5281/zenodo.22124886)

## 24장 복원 가능한 renderer와 metric faithfulness

경로동등성을 양자 renderer에 적용하면 새로운 문제가 생긴다. 일반적인 양자채널은 가역적이지 않다. 완전히 양이고 trace를 보존하는 CPTP map이라도 서로 다른 두 상태를 더 비슷하게 만들 수 있으며, 위치를 구별하는 정보와 metric rank를 지울 수 있다.

root fidelity는 CPTP map 아래에서 감소하지 않는다. 따라서 fidelity로 정의한 거리는 수축하고, 충분히 매끄러운 상태족에서 유도한 정보기하 metric도 출력에서 작아질 수 있다. 양자채널이라는 사실만으로 공간의 방향과 국소화가 보존되지는 않는다.

_F(Φρ, Φσ) ≥ F(ρ,σ) ⇒ g\_out ≤ g\_in_ (3.13)

WRRA v1.1은 이를 renderer 전체의 역함수로 해결하지 않는다. 물리적으로 보호해야 할 code subspace 또는 observable algebra를 지정하고, 그 부문에서만 recovery map이 존재하도록 요구한다. 복원은 미시상태 전체를 되살리는 일이 아니라 가시 현실에 필요한 논리정보를 보존하는 일이다.

_Recovery ∘ Φ = id on A\_protected_ (3.14)

이때 세 조건을 구분해야 한다. 첫째 localization rank가 보존되어야 한다. 둘째 출력 상태족이 하나의 공통으로 보정된 시공간기하에 faithful immersion을 이루어야 한다. 셋째 보호된 observable algebra가 의도된 논리적 시간발전을 포함해 recovery 뒤 복원되어야 한다.

경로동등성도 recovered path equivalence로 바뀐다. 서로 다른 두 경로의 raw output이 같을 필요는 없다. 각 경로의 적절한 recovery를 거친 뒤 보호된 관측대수에서 같은 물리내용과 같은 의도된 전이가 얻어져야 한다.

_R₁∘Φ\_γ₁ ≃ R₂∘Φ\_γ₂ on A\_protected_ (3.15)

여기서 불변량과 물리적 전이를 혼동하면 안 된다. flavor mixing과 decay는 원래 상태를 그대로 보존하지 않는다. renderer가 보존해야 하는 것은 변화가 없다는 사실이 아니라, 허용된 sector-changing evolution과 그 확률·전하·국소 기록이 올바르게 구현된다는 점이다. 이를 위해 Fock 공간이나 direct-sum sector가 필요할 수 있다.

### 관련 공개 연구

**Recoverable Rendering and Metric Faithfulness in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22125506](https://doi.org/10.5281/zenodo.22125506)

## 25장 시간에 걸쳐 같은 현실을 유지하기

한 시점에서 복원 가능한 renderer가 시간에 걸쳐서도 같은 현실을 유지한다고 곧바로 결론 내릴 수는 없다. 매 단계의 양자채널이 개별적으로 복원 가능해도 작은 오차가 반복되어 누적되면 보호된 관측대수와 국소 기하가 장시간 뒤에는 달라질 수 있다. snapshot recoverability와 long-time stability는 서로 다른 문턱이다.

가장 직접적인 충분조건은 각 단계의 교란 크기 ε\_k가 합산 가능하다는 것이다. n단계까지의 누적오차가 각 단계 오차의 합으로 제어되고 그 무한합이 유한하면, 반복된 rendering 뒤에도 오차를 시간에 무관한 범위 안에 둘 수 있다. 이것은 단계마다 작다는 말보다 강한 조건이다.

_‖E\_n‖ ≤ Σ\_(k=1)^n ε\_k, Σ\_(k=1)^∞ ε\_k < ∞_ (3.16)

v1.2는 시간균일 복원을 위한 세 가지 충분 메커니즘을 구분한다. 교란의 총합이 유한한 summable disturbance, 보호된 관측대수가 정확히 보존되는 noiseless observable algebra, 그리고 recovery 뒤 상태가 끌개 code manifold로 수축하는 contractive recovery다. 세 메커니즘은 서로 대체되거나 함께 사용될 수 있다.

수축 복원에서는 현재 오차가 매 단계 λ배 이하로 줄고 새 교란 ε\_k가 더해진다. 0 이상 1 미만인 λ가 시간에 무관하게 유지되면 과거의 오차는 기하급수적으로 잊히며, 제한된 새 교란 아래에서 상태는 code manifold 주변에 머문다. 다만 의도된 논리적 시간발전까지 정지시키는 복원이어서는 안 된다.

_d\_(k+1) ≤ λd\_k + ε\_k, 0 ≤ λ < 1_ (3.17)

한 시점의 metric rank가 3이라는 사실도 지속적인 3차원 공간을 보장하지 않는다. 모든 시점의 유효 metric이 하나의 공통 기준 metric에 대해 위아래로 균일하게 제한되는 uniform ellipticity가 필요하다. 또한 probe마다 달라질 수 있는 quantum Fisher 또는 Bures metric을 곧바로 공유 시공간기하와 동일시해서는 안 된다. 보손과 페르미온의 characteristic cone도 같은 보정된 인과구조와 양립해야 한다.

_c g\_\* ≤ g\_k ≤ C g\_\* for all k_ (3.18)

현실은 국소 영역마다 따로 복원된 뒤 단순히 붙는 것이 아니다. 겹치는 영역 U와 V에서 정의한 recovery가 교집합의 보호된 관측량에 대해 양립해야 한다. 이 quasi-local compatibility가 없으면 각 국소 관찰은 정상이어도 하나의 전역 현실로 접합되지 않는다. 기하와 양자상태의 안정성도 서로 피드백하므로 함께 제어해야 한다.

_R\_U│\_(U∩V) ≃ R\_V│\_(U∩V)_ (3.19)

복원에는 열역학적 장부도 따른다. syndrome을 읽고 정보를 지우며 기하와 물질에 되먹임을 남기는 비용을 숨겨서는 안 된다. 이 장의 결론은 이러한 조건 아래 시간균일한 WRRA 인터페이스가 충분하다는 조건부 정리다. 미시적 renderer의 유도나 우주 전체 시간에 대한 실제 구현을 완성했다는 선언은 아니다.

_L\_thermo = S\_syndrome + C\_erasure + B\_backreaction_ (3.20)

### 관련 공개 연구

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22126125](https://doi.org/10.5281/zenodo.22126125)

The WRRA Information Provision Ledger 10.5281/zenodo.22139233

## 26장 Einstein branch는 어떻게 선택되는가

Renderer path independence가 hypersurface deformation의 일관성을 요구한다고 해도 가능한 중력동역학은 추가 가정 없이 하나로 고정되지 않는다. Einstein branch를 얻으려면 Hojman–Kuchař–Teitelboim형 조건을 명시해야 한다.

핵심 가정은 국소 metric canonical variable, 표준 spatial-diffeomorphism action, 가역성, 추가적인 중력 canonical field의 부재, 운동량에 대한 기껏해야 이차 의존성, 공간 미분이 둘을 넘지 않는다는 조건이다.

이 조건 아래 Hamiltonian constraint와 momentum constraint가 hypersurface-deformation algebra를 first-class로 구현하면, 일반상대론의 Einstein dynamics가 조건부 저에너지 branch로 선택된다. 우주상수 항은 허용될 수 있으며 구체적인 값은 별도의 진공과 관측 문제다.

_Recovered path equivalence + HKT assumptions ⇒ Einstein branch_ (3.21)

따라서 올바른 논리의 방향은 ‘경로독립성 ⇒ Einstein 방정식’이 아니다. ‘경로동등성 ⇒ 일관된 deformation·gauge 구조’, 그리고 ‘그 구조 + HKT형 가정 ⇒ Einstein branch’다.

_G\_μν + Λg\_μν = 8πG T\_μν_ (3.22)

추가 scalar, higher derivative, nonlocal variable이나 다른 canonical content를 허용하면 다른 branch가 가능하다. 이것은 WRRA가 Einstein gravity를 부정한다는 뜻이 아니라 Einstein gravity의 적용범위와 선택가정을 분명하게 만든다는 뜻이다.

5차원 parent도 같은 방식으로 위치가 정리된다. 그것은 matter renderer의 카이럴·스펙트럼 dilation 후보이지 ultimate SOURCE가 아니다. 우리 우주의 저에너지 중력은 Einstein branch를 따를 수 있지만 renderer의 근본 구조는 더 넓을 수 있다.

### 관련 공개 연구

**Renderer Path Independence and the Einstein Branch of the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22124886](https://doi.org/10.5281/zenodo.22124886)

**Recoverable Rendering and Metric Faithfulness in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22125506](https://doi.org/10.5281/zenodo.22125506)

## 27장 시간·기하·빅뱅 그리고 열린 검증

WRRA에서 시간은 외부의 절대시계로 주어질 필요가 없다. 상태들 사이의 관계 변화와 clock subsystem의 상관관계로 시간을 정의할 수 있다. 그러나 source clock의 흔적이 가시 관측량에 비보편적으로 누출되면 등가원리와 경로독립성이 깨질 수 있다.

_T\_rel = T(clock correlations)_ (3.23)

기하도 미리 놓인 배경만이 아니라 상태 사이의 구별가능성에서 부분적으로 재구성될 수 있다. fidelity나 정보거리로부터 유효 metric을 복원하는 구상은 가능하지만, 그것이 Lorentzian spacetime과 Einstein dynamics를 자동으로 보장하지는 않는다. signature, locality와 constraint closure를 별도로 확인해야 한다.

중력의 물리적 자유도도 constraint를 제거한 뒤 세어야 한다. 3차원 공간 metric의 성분 수만 세어 graviton 자유도라고 부를 수 없다. first-class constraint와 gauge orbit를 제거한 뒤 3+1차원 Einstein branch에는 점마다 두 개의 전파 자유도가 남는다.

_N\_phys = ½(12 − 2×4 − 0) = 2_ (3.24)

빅뱅은 renderer의 초기 boundary나 rank-opening transition으로 해석될 가능성이 있다. 하지만 이것은 현재 열린 가설이다. Bessel common carrier의 autonomous opening과 우주론적 빅뱅을 동일시하려면 primordial spectrum, scale invariance, 비가우시안성, reheating과 표준 우주론 자료를 함께 통과해야 한다.

다음 검증은 수치를 맞추는 튜닝만으로 끝나지 않는다. 보정자료와 사후검증자료를 분리하고, pole·residue·threshold·gauge observable·flavor data·중력파와 우주론 자료 가운데 입력하지 않은 값을 예측해야 한다.

_Prediction = Output(test data not used in calibration)_ (3.25)

WRRA의 열린 가능성은 실패를 피하는 빈 공간이 아니다. anomaly-free quantum constraint closure, physical state space, renderer 간 observable equivalence, source-clock leakage bound와 독립적 저에너지 예측이 구체적인 다음 보스다. 우리 우주가 하나의 가능한 실현이라는 원칙은 유지하되, 그 실현을 설명하는 후보들은 관측 앞에서 경쟁해야 한다.

### 관련 공개 연구

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22126125](https://doi.org/10.5281/zenodo.22126125)

## 제3부의 경계와 다음 연구

제3부에서 고정한 것은 WRRA의 최소 구조와 하나의 조건부 Einstein branch다. 일반 양자 renderer에서는 raw path identity가 아니라 보호된 관측대수 위의 recovered path equivalence가 필요하며, 한 시점의 복원가능성만으로는 부족하다. 시간균일한 교란 제어, 공통 기하의 uniform ellipticity와 겹치는 영역의 quasi-local recovery가 함께 요구된다. 이 조건들은 gauge와 deformation의 일관성을 요구하지만, 그것만으로 Einstein 방정식의 유일성을 증명하지 않는다.

5차원 Einstein–scalar parent와 Bessel carrier는 가능한 국소 구현이다. 표준모형 매개변수의 수치 도출, all-loop 양자완결, 물리적 상태공간과 우주론적 빅뱅의 동일시는 여전히 열려 있다.

다음 단계의 목표는 더 많은 매개변수를 맞추는 것이 아니라, calibration set을 동결한 뒤 held-out observable을 예측하고 서로 다른 renderer runtime이 같은 관측대수를 재현하는지 시험하는 것이다.
