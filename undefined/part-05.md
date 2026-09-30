# 제5부 현실을 계산해보다

## 제5부 현실을 계산해보다

스펙트럼 시뮬레이션에서 복원 가능한 렌더링으로

## 제5부를 여는 말

제4부는 WRRA를 검증하려면 보정자료와 봉인된 예측자료를 분리해야 한다고 결론 내렸다. 제5부는 그 원칙을 실제 유한 계산에 적용한다.

하나의 양의 연속 스펙트럼을 유한 Jacobi 행렬로 옮기고, 같은 visible port에서 Euclidean resolvent와 실시간 진폭을 읽는다. 그 위에 localization metric과 syndrome recovery를 별도 factor로 붙여 최소한의 복원 가능한 rendering benchmark를 구성한다. 〔부록 D ‘유클리드·로런츠 서명’ 참조〕

이 계산은 미시적 우주 전체의 완성이 아니다. 정확히 계산된 것, 유한 표본에서 관찰된 것, 구성에 의해 보존된 것과 아직 열려 있는 것을 분리해 기록하는 것이 이 부의 목적이다.

## 36장 선언형 아키텍처에서 계산 가능한 모델로

지금까지 WRRA는 현실의 구현과 복원에 필요한 조건을 선언형 인터페이스로 정리했다. 그러나 SOURCE, RENDERER와 PHENOTYPE이라는 세 단어만으로는 실제 계산이 일어나지 않는다. 최소한 하나의 Hilbert 공간, 자기수반 Hamiltonian, 관측 포트와 복원 channel을 유한한 형태로 구성해야 한다.

제5부의 목표는 우주 전체를 컴퓨터 안에 복제하는 일이 아니다. 양의 연속 스펙트럼을 유한 Jacobi 행렬로 근사하고, 그 위에서 Euclidean resolvent와 실시간 생존진폭을 계산하며, 별도의 국소화·syndrome 층에 복원 dynamics를 붙이는 최소 existence benchmark를 만든다.

_H\_N = H\_Jacobi ⊗ H\_loc ⊗ H\_syn_ (5.1)

이 benchmark는 factorized되어 있다. 스펙트럼 simulation, localization metric과 recovery channel을 서로 다른 tensor factor에 놓는다. 따라서 각 조건을 명시적으로 통과시킬 수 있지만, 이 세 요소가 하나의 미시적 상호작용에서 자발적으로 생겨났다고 주장하지 않는다.

중심 계산 논문은 2026년 8월 27일 공개된 Finite-Jacobi Compatibility Benchmark for WRRA v1.2다. Version 1.2의 공개본에는 DOI 10.5281/zenodo.22126918이 부여됐으며, time-uniform WRRA 논문 10.5281/zenodo.22126125를 수치 benchmark로 보완한다.

계산의 성공 기준도 제한적이다. positive weights, real nodes, self-adjoint finite Hamiltonian, rank-one visible port, 유한 Euclidean 창의 수렴, 명시적 recovery gap과 bounded syndrome entropy가 함께 존재해야 한다.

_Benchmark = spectral simulation + metric corridor + recovery ledger_ (5.2)

이 구성의 의미는 ‘우주가 시뮬레이션임을 증명했다’가 아니다. WRRA의 일부 선언조건이 서로 모순되지 않고 하나의 유한 계산 장부 안에서 동시에 실현될 수 있다는 첫 구성적 증거다.

### 관련 연구

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22126125](https://doi.org/10.5281/zenodo.22126125)

## 37장 연속 스펙트럼을 유한 Jacobi 행렬로 옮기기

출발점은 threshold s₀ 위의 양의 generalized-Laguerre spectral density다. α가 −1보다 크면 밀도는 정규화 가능하며, 이 연구에서는 s₀=1, Λ²=1과 α=1/2을 사용했다. 연속체의 가중치는 양수이고 전체 적분은 1이다.

_ρ(s) = \[(s−s₀)^α e^(−(s−s₀)/Λ²)]/\[Γ(α+1)Λ^(2α+2)] Θ(s−s₀)_ (5.3)

변수 x=(s−s₀)/Λ²를 쓰면 측도는 x^αe^(−x)/Γ(α+1) 형태가 된다. 이 측도에 직교하는 generalized Laguerre polynomial의 삼항점화식은 실수 대칭 Jacobi 행렬을 결정한다.

N×N Jacobi 행렬의 대각성분은 s₀+Λ²(2n+α+1), 이웃한 비대각성분은 Λ²√((n+1)(n+1+α))다. 행렬이 실수 대칭이므로 고유값은 실수이며 unitary finite-time evolution이 정확히 정의된다.

_(J\_N)\_(nn)=s₀+Λ²(2n+α+1), (J\_N)\_(n,n+1)=Λ²√((n+1)(n+1+α))_ (5.4)

첫 기저벡터 e₀를 visible port로 선택하면 spectral theorem에 의해 각 고유값 s\_j의 가중치는 첫 성분의 제곱 w\_j가 된다. 따라서 w\_j는 음수가 아니고 합은 1이며, 하나의 rank-one collective port가 N개의 숨은 spectral node를 읽는다.

이 구조는 연속체를 N개의 독립적인 물리입자로 선언하는 것이 아니다. 목표 spectral measure의 Gaussian quadrature이자 유한 state-space realization이다. N은 자연의 입자 수가 아니라 근사 차수다.

Jacobi 구성의 가장 강한 점은 양성과 자기수반성을 사후 검사로 얻지 않는다는 데 있다. 측도와 recurrence에서 구조적으로 따라오므로, 복소 pole이나 음의 spectral weight를 임의 피팅으로 만들 위험을 차단한다.

### 관련 연구

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)

## 38장 하나의 visible port가 연속체를 읽는 법

연속 spectral target의 Euclidean 응답은 Stieltjes transform으로 읽힌다. Q²가 0 이상일 때 G\_E(Q²)는 spectral density를 Q²+s로 나눈 적분이다. 유한 Jacobi 모델에서는 같은 양이 e₀에 대한 resolvent의 대각행렬원소가 된다.

_G\_E(Q²)=∫ ρ(s)/(Q²+s) ds_ (5.5)

행렬을 대각화하면 유한 응답은 w\_j/(Q²+s\_j)의 합이다. 이 표현은 quadrature node와 weight가 단순 수치목록이 아니라 하나의 자기수반 Hamiltonian과 visible vector에서 나온다는 사실을 보여준다.

실시간 진폭도 같은 데이터가 소유한다. 연속 목표는 A(t)=e^(−it)(1+it)^(−3/2)이며, 유한 모델은 A\_N(t)=Σ\_jw\_je^(−is\_jt)다. Euclidean 응답과 실시간 진폭을 서로 다른 파라미터로 맞추지 않는다.

_A(t)=e^(−it)(1+it)^(−3/2), A\_N(t)=Σ\_j w\_j e^(−is\_jt)_ (5.6)

하나의 port가 모든 node를 읽는다는 것은 정보가 rank one으로 압축된다는 뜻이지 물질공간 전체가 한 차원이라는 뜻이 아니다. hidden Jacobi chain의 상태차원은 N이고, visible coupling만 e₀를 통해 이루어진다.

이 common-owner 구조는 WRRA의 최소계산 직관과 맞닿는다. 연속체의 각 성분에 별도 센서와 별도 전달자를 붙이지 않고, 하나의 collective boundary coordinate가 공통 spectral content를 운반한다.

그러나 이 visible port는 아직 전하·스핀·flavor를 가진 표준모형 입자가 아니다. 스펙트럼을 손실 없이 읽는 최소 인터페이스이며, 물리적 양자수의 공동 실현은 더 큰 embedding의 문제로 남는다.

### 관련 연구

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)

## 39장 Euclidean 창에서 얼마나 정확한가

유한 모델의 첫 시험은 Q²∈\[0,10]의 Euclidean window에서 이루어졌다. N=2,4,8,16,32로 Jacobi 차수를 늘리며 정확한 Stieltjes transform과 유한 resolvent의 최대 상대오차를 비교했다.

_δ\_N = max\_(Q²∈\[0,10]) |G\_(N,E)−G\_E|/|G\_E|_ (5.7)

오차는 차례로 4.089×10^(−2), 4.746×10^(−3), 1.858×10^(−4), 1.623×10^(−6), 1.763×10^(−9)였다. N=32에서는 지정한 창 안에서 10억분의 몇 수준까지 내려간다.

관측된 적합식 log δ\_N≈−0.55N−3.31은 이 유한 표본에서 빠른 수렴을 요약한다. 그러나 이것은 증명된 점근정리가 아니라 N=2부터 32까지의 empirical fit이다. 다른 창과 다른 α에서 같은 기울기를 보장하지 않는다.

_log δ\_N ≈ −0.55N − 3.31 \[empirical]_ (5.8)

node와 recurrence의 수치 일관성도 확인됐다. 고유값과 quadrature node의 차이는 차수에 따라 약 2.2×10^(−16)에서 5.7×10^(−14) 범위였다. 이는 사용한 double-precision 계산의 안정성과 일치한다.

Euclidean 수렴이 빠른 이유는 Stieltjes kernel이 양의 실수축 밖에서 매끄럽고 quadrature에 유리하기 때문이다. 이 성공을 곧바로 Lorentzian 장시간 dynamics의 정확성으로 옮기면 안 된다.

따라서 이 장의 정확한 판정은 fixed-window PASS다. 지정한 spectral density와 Euclidean window에 대해서는 유한 Jacobi resolvent가 빠르게 수렴하지만, 모든 scale과 모든 복소영역의 completion은 열려 있다.

### 관련 연구

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)

## 40장 실시간 추적창과 되돌아오는 파동

연속 스펙트럼의 진폭 A(t)는 위상혼합으로 감소한다. 하지만 유한 Jacobi 시스템은 이산 고유값의 유한합이므로 완전한 비가역 감쇠를 영원히 재현할 수 없다. 충분히 긴 시간이 지나면 recurrence와 revival이 나타난다.

계산에서는 연속 진폭과 유한 진폭의 상대오차가 1%를 넘기 전까지의 시간을 T\_1%로 정의했다. N=2,4,8,16,32에서 각각 0.43857, 0.96863, 1.69659, 2.67806, 4.02408이 얻어졌다.

_T\_(1%) = sup{T : relative error ≤ 0.01 on \[0,T]}_ (5.9)

이 자료의 경험적 적합은 T\_1%≈0.84√N−0.72다. 차수를 네 배로 늘려도 신뢰시간은 대략 두 배 정도 늘어나는 경향이다. 이 식 역시 점근정리가 아니라 사용한 다섯 차수의 benchmark 요약이다.

_T\_(1%) ≈ 0.84√N − 0.72 \[empirical]_ (5.10)

장시간 평균 survival plateau는 0.700, 0.450, 0.3236, 0.2318, 0.1650으로 감소했다. N이 커질수록 보이는 되돌아옴의 평균 크기는 작아지지만, 유한 N에서 영구적인 continuum damping이 되는 것은 아니다.

이 결과는 simulation과 realization의 경계를 분명하게 만든다. 유한 폐쇄계는 정해진 시간창에서 연속 응답을 매우 정확하게 흉내낼 수 있지만, 무한 시간의 비가역성과 열적 화살까지 소유하지 않는다.

따라서 N을 물리적 cutoff로 채택하려면 관측시간보다 긴 추적창, revival의 실험적 비가시성 또는 실제 환경과의 결합이 필요하다. 그렇지 않으면 모델은 finite-window simulator로 남는다.

### 관련 연구

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)

## 41장 recovery cycle은 무엇을 복원하는가

스펙트럼 simulation만으로는 WRRA v1.2의 복원조건을 시험할 수 없다. 이를 위해 전체 공간을 Jacobi spectral factor, localization factor와 syndrome qubit의 tensor product로 확장한다.

선택한 recovery generator는 amplitude-damping형 Lindblad 연산자다. syndrome excitation을 σ\_-로 바닥상태에 내리며, 밀도행렬의 횡성분은 κ/2, population defect는 κ의 비율로 감쇠한다.

_L\_rec(ρ)=κ\[σ₋ρσ₊−½{σ₊σ₋,ρ}]_ (5.11)

syndrome-transverse sector의 corrective gap은 Δ\_corr,N=κ/2다. 이 값은 Jacobi 차수 N과 recovery 순서에 의존하지 않는다. recovery factor가 spectral chain과 분리되어 있기 때문에 얻어지는 exact-in-construction gap이다. 다만 Jacobi sector의 unitary recurrence가 남으므로 전체 Liouvillian이 mixing이라는 뜻은 아니다.

_Δ\_(corr,N)=κ/2 \[syndrome-transverse sector]_ (5.12)

이 복원은 스펙트럼 진폭의 정상적인 시간발전을 역행시키지 않는다. syndrome factor의 오류를 제거하면서 Jacobi sector의 의도된 unitary evolution은 유지한다. 복원이 모든 변화를 원상복귀시키는 것이 아니라는 WRRA의 원칙을 따른다.

다만 factorization은 강한 가정이다. 실제 미시 renderer에서는 spectral, localization과 syndrome sector 사이에 상호작용이 있을 수 있고 그 결합이 uniform gap을 줄이거나 새로운 leakage를 만들 수 있다.

그러므로 여기서 통과한 것은 recovery channel의 존재와 정확한 gap 계산이다. simulation error와 recovery error가 하나의 coupled inequality로 장시간 제어된 것은 아직 아니다.

### 관련 연구

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22126125](https://doi.org/10.5281/zenodo.22126125)

## 42장 metric corridor와 공간의 보존

복원 가능한 상태가 있어도 localization metric이 붕괴하면 같은 공간을 유지했다고 말할 수 없다. benchmark는 localization factor에 공통 기준 metric g\_ref를 직접 배치하고 모든 N에서 g\_N=g\_ref로 둔다.

_c\_N g\_ref ≤ g\_N ≤ C\_N g\_ref_ (5.13)

이 선택에서는 uniform ellipticity 상수 c\_N=C\_N=1이고 condition number도 1이다. 따라서 차수가 증가해도 metric rank와 방향별 길이척도는 정확히 유지된다.

_g\_N=g\_ref, c\_N=C\_N=1, cond(g\_N)=1_ (5.14)

이 결과는 수치적 발견이 아니라 구성에 의한 exact statement다. metric corridor가 스펙트럼 근사와 독립된 tensor factor에 있기 때문에 automatic하게 보존된다.

동시에 이것이 3차원 공간의 기원을 설명하지 않는 이유도 분명하다. 기준 metric과 차원을 입력했기 때문이다. benchmark는 주어진 공간을 보존할 수 있음을 보였지만 SOURCE에서 세 방향이 자발적으로 열린 과정을 계산하지 않았다.

더 강한 모델에서는 g\_N을 고정하지 않고 spectral state와 recovery current의 함수로 만들어야 한다. 그때 uniform ellipticity와 common characteristic cone이 실제 dynamics 아래 유지되는지 시험해야 한다.

현재 판정은 metric preservation PASS, dynamical geometry origin OPEN이다. 이 두 문장을 함께 적어야 입력된 공간을 예측된 공간으로 오인하지 않는다.

### 관련 연구

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)

**Recoverable Rendering and Metric Faithfulness in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22125506](https://doi.org/10.5281/zenodo.22125506)

## 43장 syndrome entropy와 복원의 비용

복원은 논리적으로 가능하다는 말만으로 공짜가 되지 않는다. syndrome bit가 확률 p로 excitation되어 있다면 한 cycle에서 처리해야 할 Shannon entropy는 −p ln p−(1−p)ln(1−p)다.

_ΔS\_rec=−p ln p−(1−p)ln(1−p)_ (5.15)

benchmark의 p=0.01에서는 ΔS\_rec,N=0.0560015 nat/step이다. 이 값은 N과 무관하고 유한하다. syndrome factor를 하나의 qubit로 고정했기 때문에 얻어지는 bounded ledger다.

Landauer 하한을 적용하면 최소 열비용은 Q\_min=0.0560015 k\_BT per step이다. 이것은 실제 장치나 우주의 열방출량이 아니라, 선택한 syndrome record를 비가역적으로 지울 때 필요한 이상적 하한이다.

_Q\_min=k\_BT ΔS\_rec=0.0560015 k\_BT at p=0.01_ (5.16)

실제 비용을 계산하려면 cycle time, bath temperature, coupling efficiency, error production rate와 backreaction이 필요하다. 이 값들이 없으므로 cosmological heat budget은 아직 산출되지 않았다.

또한 entropy가 bounded라는 사실과 장시간 총비용이 bounded라는 사실은 다르다. cycle당 비용이 양수라면 무한한 cycle의 누적비용은 자원 공급과 방출 경로 없이는 계속 증가한다.

따라서 benchmark가 닫은 것은 한 cycle의 syndrome entropy 장부다. 우주가 이 복원을 얼마나 오래, 어떤 reservoir를 사용해 수행하는지는 다음 단계의 문제다.

### 관련 연구

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)

## 44장 계산된 것·결합된 것·아직 계산되지 않은 것

제5부에서 정확히 구성된 것은 positive finite-Jacobi realization, real nodes와 weights, self-adjoint Hamiltonian, rank-one visible port와 동일한 소유자에서 나온 Euclidean·실시간 응답이다.

수치적으로 확인된 것은 N=2부터 32까지의 fixed Euclidean window 오차, 1% 실시간 추적창, survival plateau와 node consistency다. 오차와 추적창의 적합식은 경험적 관계이며 점근정리로 승격하지 않는다.

exact-in-construction으로 닫힌 것은 선택한 factorized recovery의 N-uniform syndrome-transverse corrective gap, 고정 localization factor의 metric corridor와 선택한 syndrome qubit의 cycle당 bounded entropy다. 전체 Liouvillian의 mixing은 닫히지 않았다.

열린 것은 simulation error와 recovery cycle의 coupled long-time bound, 동역학적 3차원 기하의 기원, Lorentzian microcausality, 표준모형의 interacting gauge-covariant completion과 empirical prediction, 실제 열 reservoir, 중력 backreaction과 all-scale completion이다.

따라서 최종 명제는 ‘완성된 우주 renderer가 계산되었다’가 아니다. ‘WRRA의 스펙트럼 근사·국소화 보존·복원 gap·엔트로피 장부를 하나의 유한 factorized benchmark에서 동시에 실현할 수 있다’이다.

_Result₀ = minimal factorized compatibility benchmark_ (5.17)

후속 연구는 분리된 factor 사이에 실제 coupling을 켰다. 첫 off-diagonal localization–carrier 결합은 선택한 gapless benchmark에서 유한차수 corridor를 보였지만, 허용영역과 positivity boundary가 Jacobi 차수에 따라 달라졌다. 이것은 모든 gapless coupling의 no-go가 아니라 시험한 off-diagonal architecture의 실패다.

_H\_coupled = H\_Jacobi + H\_loc + V\_loc-carrier_ (5.18)

nearest-neighbor gauge-covariant derivative coupling은 유한차수 positivity를 회복하고 rank-one compressed response에 대한 exact identity를 만족했다. 그러나 carrier에 따라 principal kinetic coefficient가 갈라지면서 서로 다른 characteristic cone이 생겼다. 양성과 압축응답의 성공만으로 공통 시공간 phenotype이 보존되는 것은 아니었다.

_positivity corridor = corridor(N, coupling)_ (5.19)

이 실패에서 조건부 선택규칙이 남았다. 물리적 principal symbol이 Hermitian이고 strongly hyperbolic이며 constant multiplicity와 diagonalizability를 가진다는 base-class 가정 아래, WRRA-compatible carrier dependence는 상대적인 principal causal cone을 갈라서는 안 된다.

_P\_principal(ξ; carrier) split ⇒ multiple characteristic cones_ (5.20)

살아남은 finite-Jacobi class에서는 보편적인 kinetic geometry를 공통으로 유지하고, carrier와 배경의 차이는 lower-order gauge-covariant phenotype operator에 넣는다. representation-preserving scalar dressing은 허용되지만 chiral mass와 Yukawa는 doubled chiral representation space 위의 별도 Higgs-owned gauge intertwiner를 필요로 한다.

_∂P\_principal/∂carrier = 0, carrier dependence ∈ L\_lower_ (5.21)

따라서 현재의 전진은 finite-order local quadratic runtime PASS다. factorization은 처음으로 일부 해제됐지만 continuum domain convergence, Lorentzian microcausality, interacting BRST closure, Standard-Model completion과 empirical prediction은 여전히 열려 있다.

_Status = finite-order local quadratic runtime PASS_ (5.22)

### 제1세대 inventory audit가 닫은 것

6369개 모드와 15개 내부 성분의 tensor-product carrier는 제1세대 표준모형 inventory를 손실 없이 담을 수 있다. 알려진 표준모형 표현과 hypercharge를 대입했을 때 perturbative anomaly들과 SU(2) global anomaly 조건도 정확히 통과한다. 따라서 representation inventory의 수용 가능성과 anomaly compatibility는 더 이상 막연한 OPEN 항목이 아니다.

SM15 compatibility = capacity PASS ⊕ anomaly EXACT ⊕ mass availability PASS (5.23)

그러나 이 결과는 상류의 “왜 15인가”를 무조건적으로 증명하지 않으며, 6369개 제타 모드가 표준모형 charge를 생성했다는 뜻도 아니다. 질량 모드는 관측값에 가장 가까운 격자점을 고른 것이므로 prediction이 아니라 availability audit다. 실제 interacting operator, W± 전이, Higgs intertwiner, 세대 복제, CKM·PMNS 혼합과 pole residue는 계속 OPEN이다.

따라서 현재의 정확한 위치는 “표준모형을 담을 자리가 있고 알려진 제1세대 자료와 충돌하지 않는다”까지다. “표준모형을 처음부터 유도하고 새 질량을 예측한다”는 단계에는 아직 도달하지 않았다.

### 관련 연구

**Finite-Jacobi Compatibility Benchmark for WRRA v1.2** [10.5281/zenodo.22126918](https://doi.org/10.5281/zenodo.22126918)

**Local Covariant Nonfactorized Rendering in WRRA** [10.5281/zenodo.22127549](https://doi.org/10.5281/zenodo.22127549)

## 제5부의 결론 계산은 시작됐지만 우주는 아직 열려 있다

이 benchmark는 WRRA의 선언형 조건 가운데 일부가 실제 유한 양자모형에서 함께 존재할 수 있음을 보였다. 양의 Jacobi spectrum, fixed-window 수렴, rank-one visible port, recovery gap, metric corridor와 syndrome entropy가 하나의 계산 장부에 놓였다.

동시에 유한 폐쇄계의 recurrence, 입력된 localization metric과 factorized recovery는 한계를 분명히 한다. 이것은 영구적인 continuum damping, 3차원 기하의 발생 또는 우리 우주의 실제 열역학을 아직 계산하지 않는다.

후속 nonfactorized 연구는 factor coupling을 실제로 켜고 두 경로를 시험했다. 단순 off-diagonal 결합은 order-dependent corridor 때문에 탈락했고, gauge-covariant derivative 결합은 유한차수 positivity와 compressed response를 통과했지만 공통 causal cone을 갈랐다.

현재 살아남은 방향은 공통 principal kinetic geometry를 보존하면서 물질별 차이를 lower-order gauge-covariant phenotype operator에 두는 local quadratic runtime이다. 이제 다음 보스는 continuum convergence, Lorentzian microcausality, interacting BRST closure와 실제 입자·관측 데이터다.
