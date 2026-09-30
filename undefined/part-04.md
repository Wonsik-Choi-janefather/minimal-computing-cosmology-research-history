# 제4부 우리 우주는 어떻게 시험되는가

## 제4부 우리 우주는 어떻게 시험되는가

보정에서 예측으로

## 제4부를 여는 말

제3부까지 WRRA는 가능한 원천이 하나의 공동 현실로 구현되고 시간에 걸쳐 유지되기 위한 선언형 조건을 세웠다. 이제 질문은 구조의 아름다움이 아니라 그 구조가 실제 우리 우주의 수치와 관측을 견디는가이다.

제4부는 알려진 값을 새로운 기호로 옮기는 재표현, 관측으로 자유도를 정하는 보정, 입력하지 않은 값을 계산하는 독립예측을 분리한다. 이 구분이 흐려지면 아무리 많은 상수를 맞춰도 이론의 예측력은 알 수 없다.

우리 우주는 실현 가능한 우주의 한 가지일 뿐이라는 원칙은 유지한다. 목표는 유일성을 증명하는 것이 아니라 보편적인 renderer 조건 아래 우리 우주의 좌표를 찾고, 그 좌표에서 봉인된 관측값을 실제로 계산하는 것이다.

## 28장 우리 우주에 맞춘 값은 무엇인가

WRRA를 우리 우주에 적용하려면 먼저 무엇을 관측에서 가져왔는지 공개해야 한다. 공간이 세 방향으로 안정되어 있다는 사실, 표준모형의 게이지 구조, 입자 스펙트럼과 일부 결합상수는 현재 모델의 입력 또는 보정자료다. 이것들을 renderer의 출력이라고 다시 적는 것만으로 예측이 되지는 않는다.

우리 우주에 맞춘 모형은 보편 아키텍처와 실현 인자를 분리해야 한다. 보편부에는 SOURCE–RENDERER–PHENOTYPE 구조, 국소성·기록가능성·복원가능성 같은 조건이 들어간다. 실현부에는 경계조건, 스펙트럼 가중치, gap, mixing data와 관측 단위의 선택이 들어간다.

_U\_obs = R\_univ(S; θ\_realization)_ (4.1)

강제로 넣은 값은 실패가 아니라 장부 항목이다. 문제는 입력을 숨긴 채 출력처럼 말하는 데서 생긴다. 따라서 각 수량에는 source datum, structural assumption, calibration datum, derived consequence, held-out target 가운데 하나의 소유권을 부여해야 한다.

_θ = θ\_source ⊕ θ\_structure ⊕ θ\_cal ⊕ θ\_held-out_ (4.2)

현재 tuned universe model에서 재현된 3차원 필터와 U(1)·SU(2)·SU(3) algebra port는 구현의 호환성을 보여준다. 그러나 static identity evolution이나 형식적 gravity tensor port만으로 실제 동역학의 생성, 우주 팽창 또는 물질 함량이 도출된 것은 아니다.

우주의 나이, 팽창률과 암흑물질 비율처럼 보정에 사용하지 않기로 한 값은 봉인된 held-out set으로 남겨야 한다. 모델을 고칠 때마다 이 값을 들여다보면 독립검증의 의미가 사라진다. 먼저 calibration ledger를 동결하고 그 뒤에만 봉인을 열어야 한다.

이 장의 결론은 단순하다. tuned model은 우리 우주의 복제본이 아니라 보편 아키텍처 안에서 관측된 한 실현을 좌표화한 것이다. 그 가치의 첫 단계는 입력과 결과를 투명하게 분리하는 데 있다.

### 관련 공개 연구

**A Tuned Model of Our Universe Based on the Dimensional Filter** [10.5281/zenodo.22051682](https://doi.org/10.5281/zenodo.22051682)

## 29장 재표현·보정·예측을 구분하는 법

표준모형의 매개변수를 WRRA 기호로 옮기는 일은 re-expression이다. 같은 수치와 같은 관계를 새로운 SOURCE·RELATION·BOUNDARY 언어로 다시 기록하면 구조적 통찰은 얻을 수 있지만 새로운 수치 예측은 생기지 않는다.

보정은 제한된 관측자료를 이용해 renderer의 자유매개변수나 경계조건을 정하는 일이다. 보정된 모형이 그 자료를 잘 재현하는 것은 consistency check이지 독립예측이 아니다. 자유매개변수의 수와 보정자료의 수를 함께 공개해야 적합도의 의미가 생긴다.

독립예측은 calibration에 사용하지 않은 관측량을 사전에 정한 계산절차로 산출할 때 시작된다. 예측 후에 매개변수나 필터 구조를 바꾸었다면 그 값은 다음 버전의 calibration 자료가 되고, 새로운 held-out target을 다시 지정해야 한다.

_Prediction = O\_T(θ̂(C)) with T ∩ C = ∅_ (4.3)

세 층은 우열관계가 아니라 연구 순서다. 재표현은 서로 다른 이론 언어의 대응표를 만들고, 보정은 수치적으로 가능한 영역을 좁히며, 독립예측은 그 영역이 자연과 실제로 맞는지 시험한다. 앞의 두 층이 정확해야 세 번째 층의 실패도 해석할 수 있다.

예측력은 단순히 맞은 숫자의 개수로 재지 않는다. 사용한 독립 입력의 수, 허용 오차, 선택편향과 사후수정의 횟수를 함께 고려해야 한다. WRRA의 검증 점수는 held-out residual과 복잡도 비용을 동시에 기록하는 형태가 적절하다.

_χ²\_hold = Σ\_(i∈T) \[(O\_i^model−O\_i^obs)/σ\_i]²_ (4.4)

따라서 책 전체에서 ‘도출했다’는 말은 수식과 입력장부가 함께 있을 때만 쓴다. 관측값을 기호로 옮긴 것은 재표현, 값을 맞춘 것은 보정, 봉인된 자료를 맞힌 것만 예측이라고 부른다.

### 관련 공개 연구

**Wonsik Reality-Renderer Architecture v1.0** [10.5281/zenodo.22122349](https://doi.org/10.5281/zenodo.22122349)

## 30장 질량·전하·혼합은 어디에서 나오는가

WRRA에서 질량은 SOURCE에 미리 붙은 숫자일 필요가 없다. opening, transport, boundary matching과 self-energy dressing을 거쳐 실행된 상태의 pole 또는 threshold invariant로 나타날 수 있다. 그러나 이 구조적 소유권이 전자질량의 수치를 자동으로 계산해주지는 않는다.

_det S\_a⁻¹(p) = 0 at p² = m\_a²_ (4.5)

전자에 대해서는 spin 1/2, 전하 −1, color singlet, 양의 residue와 저에너지 Ward–Takahashi identity가 동시에 유지되어야 한다. 하전입자는 연질광자 구름 때문에 엄밀한 고립 pole보다 infraparticle threshold로 읽힐 수 있으므로, 단순 행렬 고유값만 질량으로 선언해서는 안 된다. 〔부록 D ‘Ward–Takahashi 항등식’ 참조〕

양성자는 더 어렵다. 전하와 color singlet, 스핀의 표현론적 구성은 가능하지만 질량·반지름·자기모멘트와 안정성은 QCD 동역학과 Λ\_QCD의 소유권을 통과해야 한다. 기본 carrier의 gap을 양성자질량과 바로 동일시하는 것은 허용되지 않는다.

세대와 flavor mixing도 스펙트럼의 개수만으로 끝나지 않는다. 왼손·오른손 sector의 전달, 유효 질량연산자의 특이값, 서로 다른 sector의 diagonalization mismatch가 CKM·PMNS 행렬을 만들어야 한다. 위상까지 살아 있어야 CP 구조를 논할 수 있다.

_V\_CKM = U\_uL† U\_dL, U\_PMNS = U\_eL† U\_νL_ (4.6)

전하비와 게이지 표현은 hardware 층에 가까울 수 있지만, Yukawa 크기·세대 hierarchy·혼합각은 firmware와 software 층의 영향을 받는다. RG running, threshold와 pole mass 변환은 execution 층이다. 서로 다른 층의 값을 하나의 상수표에 섞으면 무엇이 예측됐는지 알 수 없다.

첫 번째 현실적 목표는 모든 질량을 한 번에 맞추는 것이 아니다. 전자질량과 미세구조상수처럼 최소 보정값을 동결하고, 하나의 질량비나 혼합조합을 held-out으로 계산해보는 것이다. 이 작은 성공이 전 입자표의 사후 적합보다 더 강하다.

### 전자 gauge closure가 닫은 것과 남긴 것

후속 전자 benchmark는 dressed propagator와 전자–광자 vertex를 서로 독립적으로 고르지 않고, 같은 두 함수 A와 B에서 함께 만든다. 역전파함수를 S⁻¹(p)=A(p²)p̸−B(p²)로 두고 Ball–Chiu 종방향 vertex를 구성하면 다음 Ward–Takahashi identity가 대수적으로 닫힌다. 〔부록 D ‘전파자’ 참조〕

q\_μ Γ\_L^μ(p+q,p) = S⁻¹(p+q) − S⁻¹(p)

M\_C/m\_e=20인 매끄러운 carrier profile에서 bare mass는 m₀=0.9643653554130254로 보정되었다. 그 결과 물리 pole은 전자질량 단위 1에 놓이고 residue는 0.9259444250826103이다. 최대 Ward residual 5.1744×10⁻¹³, zero-transfer derivative 1.0799784가 보고되었으며 LSZ 정규화 뒤 F₁(0)=1이 된다. 여기서 전자질량과 profile 계수는 입력·보정값이고, pole과 residue 및 종방향 closure가 계산 결과다.

그러나 Ward–Takahashi identity는 vertex의 종방향 부분만 고정한다. 임의의 횡방향 항 Γ\_T^μ=iκσ^{μν}q\_ν/(2m)은 q\_μΓ\_T^μ=0을 만족하므로 같은 identity를 보존하면서 F₂(0)를 바꿀 수 있다. 따라서 최소 vertex에서 F₂(0)=0이라는 결과는 선택된 completion의 성질이지, WRRA가 전자의 이상자기모멘트 또는 g−2를 예측했다는 뜻이 아니다.

이 한계는 수치 오차가 아니라 비유일성 정리다. 영(零) 외부장에서 같은 K\[0]을 갖는 K\_λ\[A]=K\[A]+λσ^{μν}F\_{μν}/(2Λ)는 서로 다른 횡방향 vertex를 낳는다. 그러므로 zero-field kernel, 양의 spectral measure와 일치된 종방향 vertex만으로 full electromagnetic completion을 복원할 수 없다. 다음 단계에는 외부장에 대한 완전한 gauging map A↦K\[A] 또는 횡방향 계수를 소유하는 별도의 물리법칙이 필요하다.

두 점 profile의 계수 0.12를 물리적 scalar Yukawa coupling g\_R로 그대로 읽는 가정도 별도 loop 계산으로 기각된다. M\_C/m\_e=20에서 Δa\_e=2.216753837×10⁻⁶으로 계산되어 10⁻¹² 수준의 허용 복도보다 지나치게 크다. g\_R=0.12를 유지하려면 M\_C/m\_e≈61,730.7298, 즉 약 31.5443 GeV가 필요하다. 이 실패가 기각하는 것은 전자 benchmark 자체가 아니라 ‘두 점 계수=세 점 물리결합’이라는 소유권의 혼동이다.

상태 판정: pole·residue는 CALIBRATED NUMERICAL PASS, Ward–Takahashi closure는 EXACT-IN-CONSTRUCTION, F₁(0)=1은 NORMALIZED PASS, 최소 F₂(0)=0은 CONSTRUCTION CHOICE, WTI 또는 K\[0]만으로 g−2를 유일하게 정한다는 주장은 EXACT NO-GO, full transverse completion과 독립적인 g−2 계산은 OPEN이다.

#### 관련 후속 원고

### SOURCE 질량좌표 해상도와 동결된 중성미자 예측

제1세대 양자장부의 후속 역공학은 관측값을 없애는 대신 역할을 분리했다. 전자질량은 절대척도의 기준점이며, 전하·표현과 전자·위·아래 쿼크의 값은 낮은 복잡도의 정수관계를 찾는 항해자료다. 이 자료에서 전자 기준의 거친 질량간격 m₀=mₑ/23을 얻지만, 이 간격은 sub-eV 중성미자를 모두 0으로 보내므로 보편 질량양자라는 해석은 실패한다.

이 실패에서 제안된 후보는 중성미자 부문의 더 미세한 SOURCE 질량좌표 해상도다.

D\_ν=2·23⁶=296,071,778, q\_ν=mₑ/D\_ν=1.725929280 meV (4.12)

D\_ν는 우주 전체의 정보량이 아니다. 전자질량 한 구간을 이 부호화에서 약 2.96×10⁸칸으로 구별한다는 후보 분모이며, 이진 주소깊이는 log₂D\_ν≈28.14비트다. 6,369개 복소모드의 직접 저장량이나 우주의 최소 기술길이와도 동일시할 수 없다.

정상질량순서 점유수 (n₁,n₂,n₃)=(0,5,29)를 고정하면 m₁=0, m₂=8.62965 meV, m₃=50.05195 meV, Σm\_ν=58.6816 meV가 나온다. 그러나 질량제곱차는 이 점유구조를 찾는 데 사용됐으므로 독립예측이 아니다. 재조정 없이 동결된 시험대상은 절대질량, 그 합, 가장 가벼운 질량이 0인 정상순서 패턴이다.

주장 등급: 전자질량과 진동자료는 OBSERVATIONAL INPUT, D\_ν와 q\_ν는 OBSERVATION-GUIDED SOURCE-RESOLUTION HYPOTHESIS, 절대 중성미자 질량과 Σm\_ν는 FROZEN HOLDOUT PREDICTION, 우주 전체 SOURCE 크기와 부호화의 유일성은 OPEN이다. 역순서가 확인되거나 절대질량이 크게 다르면 동결된 (0,5,29) 모형은 폐기해야 한다.

#### 관련 공개 연구

Inferring a Source-Resolution Scale from the First-Generation Quantum Ledger · Version 1.0 · DOI 10.5281/zenodo.22173687

Electron Gauge Closure and Source Falsification in WRRA · Version 1.0 · DOI 10.5281/zenodo.22136262

### 원자에서 물분자로: 첫 다체 실행 경계

전자와 핵의 개별 조건을 적는 것만으로는 화학이 생기지 않는다. 물분자를 실행하려면 동일한 가시 좌표 위에서 세 원자핵과 열 전자를 함께 다루고, Coulomb 상호작용·페르미 반대칭성·전자상관 근사를 포함하는 다체 커널을 공급해야 한다. 이번 benchmark에서 WRRA는 SOURCE–RENDERER–PHENOTYPE의 소유권을 구분하고, 실제 수치 엔진은 표준 양자화학 RHF·MP2 계산이 담당한다.

입력은 산소·수소의 핵전하, 동위원소 질량, 전자수 10과 Coulomb 법칙이며, 관측된 O–H 길이·H–O–H 각도·쌍극자·진동수·회전상수·원자화에너지는 기하 최적화에서 제외했다. 0.85 Å와 1.20 Å의 서로 다른 두 결합, 120°의 비대칭 시작점에서 계산은 같은 두 결합과 굽은 물분자 형태로 수렴했다.

RHF/cc-pVDZ 결과는 결합길이 0.94628 Å와 결합각 104.6197°이며, 관측 평형각 104.4776°와의 차이는 0.1421°다. MP2/cc-pVDZ 결합길이는 0.96433 Å로 기준값과 약 0.0063 Å 차이가 난다. 이는 관측값에 맞춘 사후 fitting이 아니라 선택한 유한 basis와 표준 커널이 만든 수치 phenotype이며, 남은 오차도 그대로 공개한다.

같은 RHF Hessian과 평형기하에서 수소 질량만 중수소 질량으로 바꾼 no-refit 공격은 H₂O의 회전상수 (A,B,C)=(28.1352,14.9152,9.7477) cm⁻¹을 D₂O의 (15.6516,7.4633,5.0536) cm⁻¹로 이동시킨다. 이 여섯 값은 편집 과정에서 질량·기하로부터 독립 재계산해 원고와 일치함을 확인했다. 세 진동모드도 모두 올바른 방향으로 낮아졌다.

따라서 물의 최종 기하는 SOURCE에 원시 좌표로 저장될 필요가 없다는 구성적 존재성은 통과한다. 그러나 물을 WRRA가 독립 예측한 것은 아니다. 동일한 일입자 propagator와 종방향 Ward–Takahashi vertex는 횡방향 vertex, 비가약 이입자 커널, exchange–correlation completion과 분자 퍼텐셜을 유일하게 정하지 못한다. 물분자를 만든 다전자 법칙은 이번 실행에서 추가 firmware로 공급되었다.

검증 경계: 회전상수는 INDEPENDENT NUMERICAL PASS, 비대칭 시작점에서 굽은 기하로의 수렴·곡률·Hessian·IR 세기는 원고의 계산 패키지가 이번 첨부에 없어 REPORTED / PENDING FULL REPRODUCTION, 기하가 원시 SOURCE일 필요가 없다는 명제는 CONSTRUCTIVE EXISTENCE PASS, 일입자 자료만으로 다체 커널을 유일하게 정한다는 주장은 NO-GO, WRRA 고유의 미사용 분자 관측량 예측은 OPEN이다.

#### 관련 공개 연구

A Single-Water-Molecule Closure Benchmark for WRRA · Version 1.0 · DOI 10.5281/zenodo.22137355

### 6369개 모드에서 확인한 제1세대 수용 가능성

후속 계산은 서로 다른 두 질문을 분리한다. 상류 질문은 왜 exterior carrier와 anomaly 조건이 15개 chiral 성분을 선택하는가이고, 하류 질문은 이미 관측된 제1세대 표준모형 inventory를 6369개 유한 모드 안에 넣었을 때 압축이나 게이지 충돌 없이 운반할 수 있는가이다. 이번 audit는 두 번째 질문을 계산한다. 따라서 앞선 15성분의 조건부 도출 프로그램을 대체하지 않으며, 15를 제타 모드가 새로 발견했다고 주장하지 않는다.

H\_matter = C⁶³⁶⁹ ⊗ C¹⁵, dim H\_matter = 95,535 (4.6a)

여기서 15차원 슬롯에 항등 계량 G₁₅ = I₁₅를 놓으면 rank(G₁₅)=15는 정확하다. 이것은 C¹⁵를 공급한 뒤 열다섯 성분이 압축 없이 수용됨을 보이는 구성 결과이지, 6369가 15의 기원을 독립적으로 산출했다는 뜻은 아니다.

u\_k = kL/6369, m\_f(k) = m\_e√(1+u\_k²) (4.6b)

전자 질량을 k=0의 보정값으로 사용하고 L=141.459010651558을 넣으면, up 질량에는 |k|=189가 대응하여 2.20509390 MeV, down 질량에는 |k|=411이 대응하여 4.69257855 MeV를 준다. 기준값 2.20 MeV와 4.69 MeV에 대한 상대오차는 각각 약 0.2315%와 0.0550%다. 이는 유한 격자 안에 가까운 모드가 존재한다는 numerical existence pass이며, 관측값을 보지 않은 사전예측은 아니다.

질량의 소유자는 k 하나가 아니라 다음처럼 적어야 한다.

owner\_mass = (sector, phenotype map, |k|) (4.6c)

질량식은 ±k를 구분하지 못하므로 부호에 따른 이중 degeneracy가 남는다. 또한 전자와 중성미자가 모두 k=0을 사용할 수 있어도 서로 다른 sector map을 가지므로 같은 질량을 뜻하지 않는다. 이 구분은 뒤의 세대·혼합·pole residue 문제에도 그대로 이어진다.

제1세대의 왼손 Weyl inventory는 Q\_L ⊕ u\_R^c ⊕ d\_R^c ⊕ L\_L ⊕ e\_R^c로 쓰며, 색과 약한 성분을 세면 6+3+3+2+1=15다. 알려진 표준모형 hypercharge를 입력하면 SU(3)³의 2−1−1=0을 포함해 SU(3)²U(1), SU(2)²U(1), U(1)³, 중력²U(1) anomaly가 모두 0이고, SU(2) doublet 수도 짝수다. 이 산술은 exact regression test이지만, charge 표 자체가 제타 스펙트럼에서 나온 것은 아니다.

다음 단계의 통합 연산자는 공통 principal cone과 gauge covariance를 보존하면서 Higgs형 하위차수 질량 intertwiner를 포함해야 한다. 특히 W± 작용이 서로 다른 모드 소유자를 가진 u\_L과 d\_L을 일관되게 연결하고, BRST closure와 dressed-pole 조건을 함께 만족해야 한다. 그 전까지 interacting Standard-Model completion은 열린 문제다.

**상태 판정:** inventory capacity는 CONSTRUCTED, anomaly 산술은 EXACT, up/down 모드 가용성은 NUMERICAL EXISTENCE PASS, 제타에 의한 charge·세대·질량의 독립 예측은 OPEN이다.

### 관측에서 동결한 제1세대 양자장부

다음 연구노트는 제1세대 표준모형의 15개 왼손 Weyl 성분을 하나의 공통 정수 장부로 다시 적는다. 오른손 입자는 왼손 반입자장으로 바꾸며, Q\_L⊕u\_Rᶜ⊕d\_Rᶜ⊕L\_L⊕e\_Rᶜ의 성분수는 6+3+3+2+1=15다. 이 15는 새로 예측한 수가 아니라 표준모형 inventory의 압축 좌표다.

q\_Q=|e|/3, q\_Y=1/6, q\_T=1/2, q\_s=ℏ/2 (4.6d)

이 단위를 쓰면 전기전하 Q/q\_Q는 정수, 초전하 Y/q\_Y와 약한 아이소스핀 T₃/q\_T도 정수로 기록된다. 이것은 표준모형의 알려진 표현을 다른 표기법으로 옮긴 재표현이지만, 15개 채널을 공통 장부에서 비교하고 anomaly·전이·질량의 소유권을 추적하는 데 유용하다.

질량에서는 전자질량 m\_e=0.51099895069 MeV를 최초 절대기준으로 놓고 가장 단순한 제1세대 정수격자를 탐색한다. m₀=m\_e/23=22.217345682 keV로 동결하면 전자·업·다운 질량양자수는 각각 (23,99,211)이 되고, 계산값은 0.51099895069, 2.19951722, 4.68785994 MeV다.

m\_e=23m₀, m\_u≈99m₀, m\_d≈211m₀ (4.6e)

업·다운 질량은 재규격화 척도와 scheme에 따라 달라지므로 이 관계는 무척도 정리가 아니다. 관측값에서 발견해 고정한 낮은 정수 근사이며, 공통 renormalization scale의 Yukawa 장부에서 다시 시험해야 한다.

중성미자는 같은 22.2 keV 격자에 들어가지 않는다. 그래서 더 미세한 하위격자 q\_ν=m\_e/(2·23⁶)=1.725929280 meV를 두고, 정상질량순서의 정수 삼중항을 (n₁,n₂,n₃)=(0,5,29)로 동결했다. 여기서 정상질량순서는 세 질량상태가 가벼운 것부터 ν₁,ν₂,ν₃ 순으로 놓이는 경우를 뜻한다. 전자중성미자 ν\_e 자체는 이 세 질량상태의 PMNS 혼합이므로 하나의 질량정수로 적지 않는다.

m₁=0, m₂=5q\_ν=8.62965 meV, m₃=29q\_ν=50.05195 meV (4.6f)

Σm\_ν=58.6816 meV, Δm²₂₁=7.44708×10⁻⁵ eV², Δm²₃₁=2.50520×10⁻³ eV² (4.6g)

정수 삼중항과 하위격자는 NuFIT 6.0의 질량제곱차 중심값을 보며 발견한 관계다. 따라서 두 질량제곱차를 맞춘 사실 자체는 블라인드 예측이 아니다. 그러나 관계식·기준값·정수와 날짜를 2026년 8월 28일에 동결했으므로, 아직 직접 확정되지 않은 절대질량 (0, 8.62965, 50.05195) meV와 질량합 58.6816 meV는 이후 측정에 제출된 수치 후보가 된다.

검증조건은 분명하다. 정상질량순서와 약 58.68 meV의 질량합이 지지되면 후보는 살아남고, 역질량순서가 확정되거나 절대질량·질량합이 유의하게 어긋나면 이 격자후보는 폐기 또는 수정된다. 측정 결과에 맞춰 23, 5, 29를 다시 고치면 예측이 아니라 새 적합이 된다.

상태 판정: 15성분 전하장부는 STANDARD-MODEL RE-EXPRESSION, (23,99,211)은 OBSERVATION-GUIDED CALIBRATED RELATION, 중성미자 질량제곱차의 근접성은 FIT RESULT, 동결된 절대질량과 Σm\_ν=58.6816 meV는 FROZEN PHENOMENOLOGICAL PREDICTION, 이 정수격자의 WRRA 상류 유도는 OPEN이다.

#### 관련 후속 원고

An Anomaly-Free First-Generation SM Inventory in a 6369-Mode Zeta-Seeded WRRA Carrier · Version 1.0 · DOI 10.5281/zenodo.22134763

A Quantum-Property Ledger for the 15 First-Generation Components and a Frozen Neutrino-Mass Prediction · Version 1.0 · DOI 10.5281/zenodo.22140351

### 관련 공개 연구

**A Stabilized Local Standard-Model Parent for the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22123134](https://doi.org/10.5281/zenodo.22123134)

## 31장 중력과 초기우주에 닿는 지점

WRRA의 path equivalence와 복원조건은 일관된 기하를 요구하지만 우주론의 수치를 직접 주지는 않는다. Einstein branch를 선택해도 우주상수, 초기상태, 물질함량과 섭동 스펙트럼은 별도의 동역학·경계문제다.

rank-opening transition을 빅뱅 후보로 해석하려면 단순히 채널이 열렸다는 사실을 넘어야 한다. 배경 팽창, 에너지 전달, reheating에 해당하는 과정과 scalar·tensor perturbation이 같은 미시모형에서 계산되어야 한다.

_H² = (8πG/3)ρ + Λ/3 − k/a²_ (4.7)

Bessel common carrier가 primordial scale invariance와 연결될 가능성은 전달조건의 후보를 제공한다. 그러나 spectral index, tensor-to-scalar ratio, running과 비가우시안성을 입력하지 않고 계산하기 전에는 관측우주론의 예측이라고 부를 수 없다.

_P\_ζ(k) = A\_s(k/k\_\*)^(n\_s−1)_ (4.8)

시간균일 복원도 우주론적 자원장부를 필요로 한다. 무한한 시간 동안 syndrome 제거와 error correction이 지속된다면 그 엔트로피와 에너지 비용이 어디로 가는지, 기하에 어떤 backreaction을 남기는지 보여야 한다.

우주의 나이와 현재 팽창률은 좋은 held-out observable이다. 먼저 미시 매개변수와 초기조건을 동결한 뒤 Friedmann branch를 적분하고, 결과가 관측범위에 들어오는지 확인해야 한다. 값을 보고 초기조건을 다시 고치면 보정 단계로 되돌아간다.

WRRA가 초기우주에 주는 현재의 가장 강한 기여는 완성된 숫자보다 질문의 분해다. opening의 존재, 물질생성, 기하정착, 섭동생성, 장시간 안정성과 관측 matching을 서로 다른 보스로 분리함으로써 한 단계의 성공이 전체 우주론의 성공으로 과장되는 것을 막는다.

### 관련 공개 연구

**Transport Conditions for Primordial Scale Invariance in a Bessel Common-Carrier Cosmology** [10.5281/zenodo.22063222](https://doi.org/10.5281/zenodo.22063222)

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22126125](https://doi.org/10.5281/zenodo.22126125)

## 32장 독립예측을 만드는 실험 설계

독립예측은 계산이 끝난 뒤 선언할 수 없다. 먼저 calibration set C, validation set V와 최종 test set T를 나누고, T의 값은 모델과 분석규칙이 동결될 때까지 사용하지 않아야 한다. 이 원칙은 기계학습의 평가와 물리학의 blind analysis가 공유하는 최소 규율이다.

_D = C ⊔ V ⊔ T_ (4.9)

다음으로 prediction map을 고정한다. 어떤 SOURCE 입력에서 어떤 renderer를 거쳐 어떤 observable을 읽는지, renormalization scale과 단위 변환, 허용 오차를 사전에 적는다. 중간에 선택 가능한 분기가 많다면 분기 자체가 자유매개변수다.

WRRA의 첫 blind test는 거대한 목표보다 작은 비율이 적절하다. 이미 보정한 절대단위가 소거되는 질량비, 결합상수 비, residue ratio 또는 제한된 에너지창의 pole spacing이 후보가 될 수 있다.

예측은 점값일 필요가 없다. 이론 오차와 수치 오차를 분리한 구간예측도 정당하다. 다만 관측 후 구간을 넓히거나 observable을 바꾸면 사전예측이 아니다. 실패한 예측도 버전 DOI와 함께 남겨야 한다.

_O\_pred = μ\_model ± (σ\_theory ⊕ σ\_numeric)_ (4.10)

서로 다른 runtime이 같은 저에너지 관측대수를 재현한다면 공통예측과 구현특이적 예측을 분리할 수 있다. 모든 runtime에 공통인 결과는 WRRA 아키텍처의 시험이고, 한 runtime에만 나타나는 결과는 그 미시 구현의 시험이다.

이 절차가 정착되면 연구의 목표도 달라진다. 더 많은 상수를 한꺼번에 맞추는 대신, 적은 입력으로 하나의 봉인된 값을 계산하고 실패 원인을 정확한 층에 귀속시키는 것이 다음 진전이 된다.

### 실패한 공통 쌍극자에서 동결된 중성자 전류로

중성자 자기 폼팩터 연구는 이 절차를 실제 관측자료에 적용한 사례다. 양성자 자기반지름으로 고정한 공통 쌍극자 모형은 정적 반지름 비교를 통과했지만, 2024년에 공개된 유한 운동량전달 10개 점에는 χ²≈61.7로 실패했다. 여기서 닫힌 것은 공통 정적기하 전체가 아니라 “보정되지 않은 같은 쌍극자가 유한 운동량 중성자 전류까지 실행한다”는 주장이다.

누락층을 전류 dressing으로 국소화하고 다음 전이인자를 시험했다.

T(Q²)=1+a·Q²/(Q²+λ\_π)+b·Q²/(Q²+λ\_m), λ\_π=4m\_π² (4.18)

처음 다섯 점으로 두 매개변수를 맞춘 뒤 λ\_m≈0.14885 GeV²가 (m\_ρ/2)²=0.150257 GeV²에 가깝다는 사실을 사후에 인식했다. 따라서 ρ-half 척도는 독립예측이 아니라 사후 압축이다. 두 척도를 고정하고 중성자 반지름 제약으로 a를 정하면 연속 보정량은 b=0.487160 하나만 남는다.

동결된 모형은 손대지 않은 위쪽 다섯 점에서 χ²=2.751(점당 0.550)을 얻었고, leave-one-out 재적합에서는 열 점 모두 결합 인용오차 1σ 안에 들었다(max|z|=0.953). 이것은 단순한 전구간 시각적 적합보다 강하지만, 같은 자료를 나눈 회고적 ordered holdout이다. 다른 실험이나 미리 선언한 새 Q² 구간에 λ\_π, λ\_m, a, b를 바꾸지 않고 적용하기 전에는 외부 독립예측으로 올려 부를 수 없다.

동결 카드: λ\_π=0.077919575 GeV², λ\_m=0.150257017 GeV², b=0.4871600738, a=−0.2600650101. 다음 자료에서는 잔차벡터·공분산·χ²와 관측량 정의의 차이를 모두 공개하고 재조정하지 않는다.

주장 등급: 무보정 공통 쌍극자는 REJECTED, 한 진폭 runtime은 INTERNAL ORDERED-HOLDOUT PASS, ρ-half 해석은 POST-HOC COMPRESSION, 다른 실험으로의 이전성과 궁극 SOURCE에서의 유도는 OPEN이다.

### 관련 공개 연구

**A Tuned Model of Our Universe Based on the Dimensional Filter** [10.5281/zenodo.22051682](https://doi.org/10.5281/zenodo.22051682)

## 33장 무엇이 WRRA를 깨뜨릴 수 있는가

반증 가능성은 이론 전체를 한 번에 무너뜨리는 단일 실험만을 뜻하지 않는다. WRRA는 아키텍처, 구현 chassis와 우리 우주의 수치실현으로 층이 나뉘므로 실패도 정확한 소유자에게 귀속되어야 한다.

보호된 관측대수에서 두 renderer 경로가 서로 다른 gauge-invariant 결과를 내고 어떤 recovery로도 일치하지 않는다면 path-equivalence 구현은 실패한다. 반복 과정에서 오차가 무제한 누적되거나 localization rank가 붕괴하면 time-uniform renderer 후보도 실패한다.

_sup\_n ‖E\_n‖ = ∞ ⇒ time-uniform candidate FAIL_ (4.11)

보손과 페르미온이 보정으로 제거할 수 없는 서로 다른 characteristic cone을 보인다면 공통 시공간 phenotype 조건이 깨진다. 겹치는 영역의 recovery가 교집합에서 모순된 값을 내놓는다면 quasi-local gluing도 실패한다.

입자 부문에서는 음의 spectral density, Ward identity 위반, gauge anomaly, 잘못된 pole·threshold 구조 또는 flavor data와의 독립적 불일치가 해당 구현을 폐쇄한다. 유한 창에서의 비슷한 곡선이나 양의 상관만으로 이런 실패를 덮을 수 없다.

우주론 부문에서는 opening 뒤 재폐쇄, scale invariance 실패, 과도한 backreaction, 관측과 양립하지 않는 expansion history가 반증자가 된다. 단, 관측값을 다시 입력해 맞춘 버전은 원래 예측의 성공이 아니라 새 calibration model이다.

_O\_T ∉ I\_pred ⇒ frozen model FAIL_ (4.12)

가장 중요한 fail-closed 규칙은 침묵이다. 필요한 계산이 정의되지 않았거나 수치적으로 불안정하면 ‘맞았다’와 ‘틀렸다’ 어느 쪽도 선언하지 않는다. OPEN은 성공의 완곡어가 아니라 아직 판정할 수 없다는 독립된 상태다.

### 관련 공개 연구

**A Fail-Closed Verification Methodology for Exploratory Riemann-Hypothesis Computation** [10.5281/zenodo.21961236](https://doi.org/10.5281/zenodo.21961236)

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22126125](https://doi.org/10.5281/zenodo.22126125)

## 34장 우리 우주는 특별하지 않다

이 책은 우리 우주의 유일성을 증명하려 하지 않는다. 보편적인 최소계산 원리와 renderer 조건이 여러 실현을 허용하고, 우리 우주는 그 가운데 관찰자와 안정된 기록이 가능한 한 사례일 수 있다.

비특권 원리는 모든 우주가 같은 상수를 가져야 한다는 뜻이 아니다. 공통인 것은 생성과 구현의 법칙 또는 허용조건이며, 경계조건·스펙트럼·차원·결합과 관측가능한 phenotype은 달라질 수 있다.

_Law\_univ + θ\_i → U\_i_ (4.13)

따라서 유일성 증명보다 실현공간의 지도를 그리는 편이 더 자연스럽다. 매개변수 공간의 어떤 영역에서 국소성, 장시간 복원, 안정된 물질과 인과구조가 함께 가능한지 찾고, 우리 우주의 좌표가 그 안에 놓이는지 묻는다.

_M\_viable = {θ : locality ∧ stability ∧ recordability}_ (4.14)

관찰자 선택효과는 설명을 대신하지 않는다. 우리가 존재하므로 가능한 영역에 있다는 말은 그 영역의 크기와 구조, 전이확률을 계산해주지 않는다. selection condition과 dynamical probability를 구분해야 한다.

다른 실현 가능한 우주는 우리 우주의 복제나 평행세계 서사를 요구하지 않는다. 수학적으로 허용되는 서로 다른 renderer family, 초기조건과 phenotype의 집합으로 다룰 수 있다. 실제 공존 여부는 추가 존재론이고 이 책의 최소 주장 밖에 있다.

우리 우주가 비특권적이라는 태도는 연구를 약하게 만들지 않는다. 오히려 우리 우주에만 맞는 특별 규칙을 추가하지 못하게 하고, 같은 법칙이 다른 입력에서도 일관된 우주를 만드는지 시험하게 한다.

### 관련 공개 연구

**The Coexistence of All Possible Universes and the Accidental-Location Hypothesis** [10.5281/zenodo.22042020](https://doi.org/10.5281/zenodo.22042020)

**The Universal Minimum-Computation Model and the Non-Special Universe** [10.5281/zenodo.22067717](https://doi.org/10.5281/zenodo.22067717)

## 35장 현재 닫힌 것과 열린 가능성

현재 닫힌 것은 하나의 완성된 만물이론이 아니다. 가능한 우주를 유일성 없이 다루는 관점, 최소계산과 차원필터의 운영 직관, SOURCE–RENDERER–PHENOTYPE의 선언형 구조, recovered path equivalence와 시간균일 복원의 충분조건이 연구계보로 고정되었다.

_Ledger = EXACT ⊕ CONDITIONAL ⊕ WORKING ⊕ OPEN ⊕ FAIL-CLOSED_ (4.15)

조건부로 닫힌 것은 명시한 가정 아래의 결과다. HKT형 가정 아래 Einstein branch가 선택되는 논리, 특정 spectral target을 재현하는 양자 runtime, 제한된 부문에서의 BRST와 recovery 조건이 여기에 속한다. 가정을 제거하면 결론도 자동으로 유지되지 않는다.

구조적으로 가능하지만 수치가 열려 있는 부분도 있다. 표준모형의 국소 parent, chiral matter와 15채널 carrier, 질량·결합의 보편 생성자, autonomous opening과 spectral settlement는 후보구조를 가졌지만 우리 우주의 전체 상수표를 독립적으로 산출하지 않았다.

실패로 닫힌 경로도 지식이다. 단순한 log-det 에너지, democratic rank-one opening의 14개 dark direction, 유한 인과제어의 exact echo와 full-rank Gram만으로 질량을 정하는 도약은 폐기되거나 제한되었다. 이 기록은 같은 막힌 길을 다시 정답처럼 포장하는 것을 막는다.

다음 연구의 최우선 순위는 유일성 증명이 아니라 blind prediction이다. calibration ledger를 동결하고, 최소 하나의 held-out 입자 또는 우주론 observable을 계산하며, 실패하면 어느 층의 가정이 책임지는지 기록해야 한다.

_Next boss = one frozen calibration + one held-out prediction_ (4.16)

열린 가능성은 이 책의 마지막 빈칸이 아니다. 여러 가능한 우주 가운데 우리 우주라는 한 실현이 어떻게 공동의 현실로 나타나고 시간에 걸쳐 유지되는지를 묻는 연구 프로그램의 출구다. 이 책은 그 답을 완성했다기보다, 무엇을 계산해야 답이 되는지를 분명히 남긴다.

### 정보 제공 원장이 새로 닫은 경계

정보 제공 원장은 올바른 우주 SOURCE를 찾아내지 않았다. 대신 어떤 물리 질문에도 ‘누가 정보를 소유하는가, 무엇을 실제로 읽는가, 어떤 계산을 거치는가, 언제 관측형으로 실현되는가, 어떤 기록이 남는가’를 요구하는 감사 구조를 닫았다.

이제 우주 크기·질량·모양을 묻는 질문도 모호한 하나의 숫자로 답하지 않는다. 관측가능 우주의 반지름은 관측자와 현재 인과상태에서 얻는 OBSERVED/DERIVED이고, 우주 전체 크기는 전역 위상과 기하가 유한한 경우에만 CONDITIONAL하며, 총질량은 영역과 중력적 정의가 고정된 경우에만 계산 가능하다. 미래의 구체적 기하는 부트 패키지에 완성본으로 들어 있지 않고 열린 실행을 통해 생성된다.

다음 구현목표도 더 선명해졌다. LAW HEADER와 SOURCE v0.2를 받아 하나의 전자 상태를 만들고, 전하 표현·질량 보정·공간확률·광자 vertex·단일 검출사건의 제공경로를 끝까지 출력하는 provision trace compiler가 첫 실행과제가 된다.

### 관련 공개 연구

**Wonsik Reality-Renderer Architecture v1.0** [10.5281/zenodo.22122349](https://doi.org/10.5281/zenodo.22122349)

**Time-Uniform Recoverable Rendering in the Wonsik Reality-Renderer Architecture** [10.5281/zenodo.22126125](https://doi.org/10.5281/zenodo.22126125)

## 제4부의 결론 보정이 끝나는 곳에서 이론이 시작된다

WRRA는 현재 우리 우주의 모든 상수를 계산하는 완성된 이론이 아니다. 그러나 무엇이 입력이고 무엇이 구조적 귀결이며 무엇을 아직 계산해야 하는지 구분하는 검증 가능한 연구 프로그램으로 진입했다.

다음 진전은 더 넓은 사후 적합이 아니라 더 좁은 사전예측이다. calibration set을 동결하고 하나의 held-out observable을 선택한 뒤, 결과가 맞든 틀리든 계산규칙과 버전을 공개해야 한다.

우리 우주가 유일하지 않더라도 이 시험은 가능하다. 보편법칙이 여러 우주를 허용한다면, 그 법칙이 우리 우주라는 한 실현을 얼마나 적은 입력으로 재구성하고 새로운 값을 예측하는지가 바로 검증의 기준이다.
