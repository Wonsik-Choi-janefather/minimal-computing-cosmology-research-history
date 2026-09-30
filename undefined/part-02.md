# 제2부 가능성에서 현실로

## 제2부 가능성에서 현실로

최소계산과 차원필터의 탄생

## 제2부를 여는 말

제1부가 우주의 다양한 가능성을 열었다면, 제2부는 그 가능성이 어떻게 하나의 현실로 좁혀지고 구현되는지를 묻는다. 이 과정은 한 번에 완성된 이론이 아니라 여러 가설과 실패, 보수와 재정의를 거쳐 형성된 연구 계보다.

소수의 독립성에서 관계의 문법을 찾고, 차원필터로 가시 방향을 나누며, Hamiltonian과 공통전달자로 동역학과 내부 채널을 연결했다. 마지막에는 SOURCE와 관측 가능한 대상 사이의 누락된 층을 RENDERER라 부르게 되었다. 〔부록 D ‘해밀토니안’ 참조〕

각 장은 확정된 정리와 직관적 제안, 보정된 모델과 열린 문제를 구분한다. 이 부의 목적은 WRRA를 이미 완성된 만물이론으로 선언하는 것이 아니라, 왜 이런 아키텍처가 필요해졌는지를 재현 가능한 순서로 보여주는 데 있다.

## 9장 모든 가능성을 한꺼번에 실현할 필요가 있는가

가능한 우주의 공간을 열었다고 해서 그 모든 가능성이 동시에 물리적 현실이 되어야 하는 것은 아니다. 수학은 수많은 상태를 허용할 수 있지만, 관측자는 언제나 일정한 지속성과 국소성을 가진 한 현실 안에서 사건을 경험한다. 가능성의 집합과 실현된 현실 사이에는 선택과 압축의 문제가 남는다.

여기서 선택은 외부의 설계자가 후보를 고른다는 뜻이 아니다. 서로 양립할 수 없는 관계를 제거하고, 보존 가능한 구조를 남기며, 한정된 자원 안에서 일관된 상태를 갱신하는 과정이다. 현실은 모든 답을 미리 계산해 저장한 목록이라기보다 필요한 관계를 필요한 순간에 구현하는 과정일 수 있다.

_R = Π\_constraints(S\_possible)_ (2.1)

이 생각은 우주를 거대한 컴퓨터라고 단정하는 시뮬레이션 우주론과 다르다. 최소계산 우주론은 우주 밖의 프로그래머나 기계를 가정하지 않는다. 계산이라는 말도 디지털 명령어에 한정하지 않는다. 상태의 구별, 관계의 전파, 제약의 적용, 관측 가능한 결과의 갱신을 묶어 부르는 기능적 언어다.

핵심 질문은 무엇이 계산되는가가 아니라 무엇을 굳이 계산하지 않아도 되는가이다. 모든 가능한 경로의 세부를 독립적으로 실재화하지 않고도, 경계에서 필요한 일관성과 보존량을 유지할 수 있다면 현실은 훨씬 적은 표현 비용으로 작동할 수 있다.

_C\_realized ≪ C\_enumerated_ (2.2)

양자역학은 이 직관을 자극한다. 측정 전 상태는 고전적 속성의 완성된 목록이라기보다 가능한 결과의 진폭으로 기술되고, 상호작용은 특정 기저에서 기록 가능한 결과를 남긴다. 그러나 이 책은 표준 양자역학의 해석 문제를 이미 해결했다고 주장하지 않는다. 다만 가능성과 기록 사이에 구현 층이 필요하다는 구조적 질문을 꺼낸다.

따라서 최소계산은 게으른 우주가 아니라 중복을 피하는 우주라는 뜻이다. 같은 관계를 여러 번 독립적으로 생성하지 않고, 공통 전달과 제약을 통해 다수의 현상을 함께 조직한다. 이후의 차원필터와 공통전달자 연구는 이 압축을 물리적 구조로 바꾸려는 시도였다.

### 관련 연구

**34. The Coexistence of All Possible Universes and the Accidental-Location Hypothesis** [10.5281/zenodo.22042020](https://doi.org/10.5281/zenodo.22042020)

**55. The Universal Minimum-Computation Model and the Non-Special Universe** [10.5281/zenodo.22067717](https://doi.org/10.5281/zenodo.22067717)

## 10장 최소계산 우주론

최소계산 우주론의 첫 원칙은 현실이 관측되지 않은 모든 세부값을 고전적으로 확정해 보관해야 할 이유가 없다는 것이다. 필요한 것은 아무것도 없는 상태가 아니라, 가능한 상태와 실제 기록 사이를 잇는 일관된 규칙이다. 따라서 최소화의 대상은 계산방식만이 아니라 소스데이터의 크기, 그 데이터를 읽는 순서, 시간 진화와 현실 재현 조건까지 포함한다.

둘째 원칙은 계산량의 최소화가 단순히 연산 횟수의 최소화를 뜻하지 않는다는 것이다. 표현해야 할 독립 자유도, 전달해야 할 정보, 유지해야 할 제약과 수정 때 다시 계산해야 할 범위뿐 아니라, 최초 적재와 선택적 출력의 비용도 함께 줄이는 구조적 최소화다.

C\_min = min\[L\_source + C\_read + C\_evolution + C\_render + C\_record] (2.3)

셋째 원칙은 국소성이다. 한 지점의 작은 변화가 우주 전체의 모든 기술을 처음부터 다시 쓰게 만든다면 안정적인 물리법칙이 되기 어렵다. 현실은 국소 상호작용과 제한된 전달을 통해 갱신되며, 멀리 떨어진 영역의 관계는 공통 규칙 아래에서 연결되어야 한다.

넷째 원칙은 재사용이다. 질량·전하·스핀·위치가 서로 무관한 네 공장에서 따로 만들어진 뒤 한 입자에 붙는다면 결합 규칙이 폭발한다. 하나의 공통 상태와 공통 전달구조에서 여러 관측량이 공동으로 드러난다면 설명 비용이 줄어든다.

_ΔR(x) → ΔR(N\_local(x))_ (2.4)

이 관점에서 법칙은 모든 사건의 완성된 대본이 아니라 구현 가능한 상태를 제한하는 압축 규칙이다. 초기조건과 경계조건, 진공과 결합상수는 한 우주 인스턴스를 지정한다. 관측값을 입력하는 일은 자연스럽지만, 입력과 구조적 도출과 새로운 예측은 반드시 구별해야 한다.

### 한 번 읽히는 우주

이 관점에서 물리법칙과 상수는 매 순간 외부에서 다시 불러오는 명령이 아니다. SOURCE에 기록된 법칙, 상수와 초기 씨앗은 우주 실행의 시작에서 한 번 읽혀 실행 가능한 상태를 구성한다. 이후의 시간 진화는 이미 적재된 규칙과 현재 상태에 의해 자율적으로 계산된다.

(laws, constants, seed) ─BOOT→ Ψ₀, Ψ(t+Δt)=T\_Δt\[Ψ(t)]

여기서 ‘한 번’은 우주 밖의 컴퓨터가 파일을 여는 장면을 문자 그대로 뜻하지 않는다. 법칙과 상수가 매 시간 단계마다 새로운 외부 입력을 요구하지 않고, 초기화된 동역학 안에서 지속적으로 효력을 갖는다는 구조적 표현이다. 이렇게 해야 우주는 외부 호출에 의존하지 않는 자기완결적 실행계가 된다.

따라서 최소계산 우주론은 저장–읽기–실행–출력–기록의 전 과정을 다룬다. 소스의 기술 길이 L\_source, 활성화 순서 C\_read, 자율 진화 C\_evolution, 관측 경계에서의 선택적 출력 C\_render와 되돌릴 수 없는 기록 C\_record가 하나의 비용 장부에 들어간다.

### 정보는 여섯 가지 방식으로 제공된다

우리가 어떤 물리량을 묻는다고 해서 그 답이 모두 SOURCE 안에 숫자로 들어 있어야 하는 것은 아니다. WRRA 정보 제공 원장은 답이 현실에 나타나는 경로를 INPUT·DERIVED·CALIBRATED·OBSERVED·OPEN EVENT·OPEN의 여섯 등급으로 나눈다. 이 구분은 이미 넣은 값을 예측이라고 부르는 오류와, 아직 발생하지 않은 사건을 미리 저장된 미래라고 부르는 오류를 함께 막는다.

I\_direct={법칙, 상수, 초기관계, 위상, 경계}, I\_derived(t)=E\_WRRA^t\[I\_direct], I\_observed(Q,t)=R\_Q\[I\_derived(t)]

예를 들어 빛의 속도와 플랑크상수는 법칙 헤더에서 한 번 읽히는 INPUT일 수 있다. 현재의 물질분포와 우주 나이는 초기상태와 동역학에서 계산되는 DERIVED다. 지금 단계의 전자질량과 일부 결합상수는 관측값으로 맞춘 CALIBRATED다. 특정 전자 검출 위치는 확률분포 안에서 사건이 일어날 때 하나의 기록으로 추가되는 OPEN EVENT다. 올바른 최종 SOURCE 자체는 여전히 OPEN이다.

핵심은 정보의 등급이 영구 신분이 아니라는 점이다. 오늘 CALIBRATED인 질량값도 훗날 같은 관측값을 다시 사용하지 않는 더 깊은 생성 규칙이 발견되면 DERIVED로 이동할 수 있다. 과학적 진전은 값을 더 많이 넣는 데 있지 않고, 입력으로 남아 있던 정보를 독립적으로 도출하는 데 있다.

### 시뮬레이션 우주론·표준모형과 무엇이 다른가

세 관점은 같은 층에서 경쟁하지 않는다. 시뮬레이션 우주론은 통일된 표준 이론이라기보다 우주가 외부 계산기에서 실행될 수 있다는 철학적·계산적 가설들의 묶음이다. 표준모형은 입자와 강력·약력·전자기력을 정밀하게 기술하는 검증된 양자장론이다. 최소계산 우주론은 이 법칙과 상수까지 포함한 우주 인스턴스가 어떤 정보 구조와 실행 순서, 선택적 출력 조건으로 현실을 구성하는지를 묻는 연구 프로그램이다.

| **구분**     | **최소계산 우주론**                     | **시뮬레이션 우주론**                     | **표준모형**                                     |
| ---------- | -------------------------------- | --------------------------------- | -------------------------------------------- |
| **성격**     | 현실 구현의 비용·순서를 묻는 연구 프로그램         | 외부 계산 실행을 상정하는 가설군                | 우리 우주의 물질 표현형과 내부 동역학을 기술하는 검증된 양자장론         |
| **핵심 질문**  | 얼마나 적은 소스와 출력으로 하나의 현실을 구현하는가    | 우리 우주는 다른 계산계의 시뮬레이션인가            | 실현된 입자·장·세 기본힘의 표현형은 어떤 대칭과 동역학으로 작동하는가      |
| **외부 실행자** | 필요하지 않다. 우주 내부의 자기완결 실행을 목표로 한다  | 대체로 상위 계산기나 실행 환경을 가정한다           | 가정하지 않는다                                     |
| **법칙·상수**  | 최초 부트 입력으로 한 번 적재되고 소유권·크기를 감사한다 | 시뮬레이터의 코드·매개변수로 볼 수 있다            | 표현형의 매개변수 일부를 관측 입력으로 받아 RG 흐름으로 계산한다        |
| **시간 진화**  | 적재된 규칙과 현재 상태에 따른 자율 계산          | 외부 계산 자원과 구현 방식에 의존               | 표현형 라그랑지안과 양자장론 규칙에 따른다                      |
| **관측**     | 기록 가능한 상호작용에서 국소 현실을 선택적으로 출력    | 필요한 장면만 렌더링한다는 비유가 가능하나 필수 명제는 아님 | 표현형의 관측가능량과 사건확률을 정밀 계산하되 측정 해석을 하나로 고정하지 않음 |
| **예측 상태**  | 현재는 구조 가설·부분 계산·경계 검증이 혼재        | 고유하고 반증 가능한 예측을 만들기 어렵다           | 다수의 정밀 예측이 실험으로 확인됨                          |
| **중력·우주론** | 통합과 초기우주 연결은 아직 OPEN             | 선택한 시뮬레이션 규칙에 따라 달라진다             | 중력을 포함하지 않으며 표현형의 궁극적 SOURCE나 완전한 우주론은 아니다   |

이 비교에서 최소계산 우주론은 표준모형을 폐기하거나 대체한다고 주장하지 않는다. 오히려 우리 우주의 renderer가 성공하려면 표준모형이 이미 설명하는 대칭, 입자 목록과 정밀 관측을 재현해야 한다. 차이는 표준모형의 매개변수를 다른 기호로 옮기는 데 있지 않고, 그 입력의 크기와 소유권, 읽기 순서, 실행과 관측 기록까지 하나의 계산 장부로 확장하는 데 있다.

최소계산이라는 이름은 아직 정리가 끝난 정리가 아니라 연구 프로그램의 이름이다. 무엇을 비용으로 셀 것인지, 양자장론과 중력에서 이를 어떻게 정의할 것인지, 엔트로피·작용·회로복잡도와 어떤 관계인지가 열려 있다. 이 책은 그 불완전성을 숨기지 않고 다음 구조로 넘어간다.

이 실행계에서 SOURCE는 물리법칙과 상수, 초기 복소 씨앗, 의존순서, 경계, SOURCE-to-state 인터페이스와 사건질의를 포함한다. 독립 항목은 병렬로 읽힐 수 있지만 하류 객체는 소유자와 해석법이 적재되기 전에 읽을 수 없다. 부트 이후 Actual 상태는 관측자가 없어도 자율적으로 진화하며, 고전적 영상은 안정적이고 공유 가능한 물리적 기록이 요구될 때 선택적으로 구성된다.

Universe = BOOT\[law, constants, schema] + EVOLVE\[Actual] + RENDER\[record query] + APPEND\[event]

관련 공개 연구: A Zeta-Seeded WRRA Open-Universe Execution Model, Version 1.1, DOI 10.5281/zenodo.22137993

관련 공개 연구: The WRRA Information Provision Ledger, Version 1.0, DOI 10.5281/zenodo.22139233

### 관련 연구

**32. The Finite-Computational Vacuum and the Cosmic Survival Selection Hypothesis** [10.5281/zenodo.22040291](https://doi.org/10.5281/zenodo.22040291)

**55. The Universal Minimum-Computation Model and the Non-Special Universe** [10.5281/zenodo.22067717](https://doi.org/10.5281/zenodo.22067717)

**57. Minimum-Computational Filter-Spectral Revision of the Fifteen-Channel Common-Carrier Model** [10.5281/zenodo.22068573](https://doi.org/10.5281/zenodo.22068573)

**58. Ground-Subtracted Lossless-Angle Completion of the Fifteen-Channel Common-Carrier Model** [10.5281/zenodo.22069630](https://doi.org/10.5281/zenodo.22069630)

## 11장 소수에서 관계의 문법으로

연구의 초기에는 소수가 독립적인 주기와 차원의 씨앗이 될 수 있다는 생각이 있었다. 합성수는 소인수의 결합으로 분해되지만 소수는 더 작은 정수 주기의 곱으로 환원되지 않는다. 이 산술적 독립성이 물리적 자유도의 독립성과 닮아 보였다.

이 직관에서 Prime Operator와 WJNS 계열의 탐색이 시작되었다. 소수마다 고유한 위상이나 주기 방향을 부여하고, 합성수를 그 방향들 사이의 결합으로 읽으면 수의 구조를 관계망으로 바꿀 수 있다. 수열은 목록이 아니라 생성과 결합의 문법이 된다.

_n = ∏ₚ p^νₚ(n) ⇒ composite = coupled prime relations_ (2.5)

그러나 산술적 비유가 곧 물리학은 아니다. 소수가 독립적이라는 사실만으로 공간차원이나 입자가 도출되지는 않는다. 리만가설과의 연관을 탐색했다고 해서 증명이 생기는 것도 아니다. 이 단계의 성과는 정답보다 연구 언어의 변화였다.

그 변화는 중요했다. 대상의 속성을 직접 부여하는 대신, 독립적인 원천과 그 사이의 관계를 먼저 놓게 되었기 때문이다. 어떤 방향이 보존되고, 어떤 조합이 중복되며, 어떤 경계에서 관측 가능한 패턴이 되는지를 묻는 방식이 생겼다.

소수 프로그램은 따라서 WRRA의 완성본이 아니라 계보의 출발점이다. 독립성은 SOURCE의 후보 언어가 되었고, 결합은 RELATION의 문법이 되었으며, 실제로 남는 패턴은 BOUNDARY 기록의 문제로 이동했다.

이 책은 그 계보를 과장하지 않는다. 소수에서 표준모형을 계산했다고 말하지 않으며, 산술이 우주를 유일하게 강제한다고도 말하지 않는다. 다만 독립 항과 결합 항을 분리하는 사고가 차원필터와 렌더러 구조를 낳았음을 기록한다.

### 관련 연구

**06. The Dimension Sieve Hypothesis: Prime Numbers as One-Dimensional Survivors and Riemann Zeta Zeros as Dimensional Portals** [10.5281/zenodo.21899807](https://doi.org/10.5281/zenodo.21899807)

**08. Arithmetic Phase Flow and the Dimensional Filter: A Resonance-Space Representation of Divisibility and Prime States** [10.5281/zenodo.21901126](https://doi.org/10.5281/zenodo.21901126)

**24. The Wonsik Filter: Infinite Parallel Number Ports with a Single Completed Heat-Flow Serial Filter** [10.5281/zenodo.21943881](https://doi.org/10.5281/zenodo.21943881)

**29. The Zeta Null State: Scalar Zeros, Nonzero Internal States, and the Observability Paradox — The Wonsik–Jeongin Null-State System (WJNS)** [10.5281/zenodo.22012524](https://doi.org/10.5281/zenodo.22012524)

## 12장 차원필터의 탄생

가능한 방향이 많을 때 관측 가능한 방향은 어떻게 생기는가. 차원필터는 이 질문에 대한 첫 구조적 답이었다. 필터는 차원을 무에서 만드는 장치가 아니라, 원천에 존재하는 관계 후보 가운데 일관되게 전달되고 국소적으로 기록될 수 있는 부분을 통과시키는 연산이다.

필터 F가 원천 상태에 작용한다고 할 때 K\_DF=F†F는 통과하는 부문의 유효 커널로, L\_DF=I−K\_DF는 통과하지 않는 보완 부문으로 읽을 수 있다. 이 표기는 아직 특정 미시이론을 완성했다는 뜻이 아니라 가시 부문과 비가시 부문의 소유권을 분명히 하는 장부다. 〔부록 D ‘커널’ 참조〕

_K\_DF = F†F, L\_DF = I − K\_DF_ (2.6)

차원필터 연구에서는 3차원 구조를 입력한 뒤 열추적과 스펙트럼 지표가 그것을 안정적으로 재구성하는 수치실험을 수행했다. 이것은 알고리즘의 회귀검사로 의미가 있지만, 3차원을 무입력으로 예측한 결과는 아니다. 입력된 구조를 되찾은 것과 자연이 왜 그것을 선택했는지는 다른 주장이다.

이 구분 때문에 유일성 증명은 연구의 필수 목표가 아니다. 우리 우주는 실현 가능한 우주들 가운데 하나일 수 있다. 차원필터의 임무는 오직 3+1차원만 가능하다고 선언하는 것이 아니라, 주어진 원천과 경계조건에서 어떤 유효 차원이 안정적으로 나타나는지 계산 가능하게 만드는 것이다.

_d\_eff(E) = −2 · d log Tr(e^(−tK\_DF)) / d log t_ (2.7)

차원은 이제 배경의 빈 상자가 아니라 관계가 지속되는 독립 방향의 수가 된다. 이 관점은 차원을 입자나 힘과 분리된 선행 무대로 두지 않고, 전달과 관측의 구조 안에서 함께 다루게 했다.

하지만 필터만으로는 충분하지 않았다. 통과하는 부분공간을 지정해도 그 위에서 상태가 어떻게 시간에 따라 움직이는지는 정해지지 않는다. 정적인 선택 연산자에서 동적인 물리학으로 건너가기 위해 Hamiltonian 다리가 필요했다.

### 차원필터에서 WRRA로

차원필터는 지금의 WRRA와 경쟁하는 별도 이론으로 남은 것이 아니다. 초기 차원필터가 맡았던 차원 선택과 표현 변환은 WRRA 내부의 첫 구현 모듈로 보존됐고, 그 위에 SOURCE의 의존순서 읽기, 공통 전달, 속성의 공동 귀속, 자율 진화, 선택적 실현과 안정된 기록 형성이 추가됐다.

Dimensional Filter ⊂ WRRA

초기의 1차원 점도 이미 보이는 물리공간의 점으로 고정하지 않는다. 그것은 SOURCE 관계구조의 최소 주소다. WRRA 내부의 차원필터가 이 주소들 사이의 허용 관계를 가시적인 3차원 기하와 표현형 방향으로 변환하고, 나머지 WRRA 모듈이 질량·전하·스핀·위치가 같은 인과구조에 귀속되도록 실행한다.

SOURCE address → dimensional selection → common transport → lawful phenotype → stable record

관련 공개 연구: A Zeta-Seeded WRRA Open-Universe Execution Model, Version 1.1, DOI 10.5281/zenodo.22137993

### 관련 연구

**08. Arithmetic Phase Flow and the Dimensional Filter: A Resonance-Space Representation of Divisibility and Prime States** [10.5281/zenodo.21901126](https://doi.org/10.5281/zenodo.21901126)

**12. Dimensional Filtering and the Weil Explicit Formula** [10.5281/zenodo.21905718](https://doi.org/10.5281/zenodo.21905718)

**31. The Hypothesis on Gravity and Three-Dimensional Space** [10.5281/zenodo.22038142](https://doi.org/10.5281/zenodo.22038142)

**37. A Tuned Model of Our Universe Based on the Dimensional Filter** [10.5281/zenodo.22051682](https://doi.org/10.5281/zenodo.22051682)

**56. Filter-Restored Revision of the Fifteen-Channel Common-Carrier Model** [10.5281/zenodo.22067895](https://doi.org/10.5281/zenodo.22067895)

**57. Minimum-Computational Filter-Spectral Revision of the Fifteen-Channel Common-Carrier Model** [10.5281/zenodo.22068573](https://doi.org/10.5281/zenodo.22068573)

## 13장 SOURCE–RELATION–BOUNDARY

차원필터의 언어가 확장되면서 세 개의 기본 항이 고정되었다. SOURCE는 가능한 독립 성분과 잠재적 상태의 저장고다. RELATION은 성분들이 어떻게 결합하고 서로를 제한하며 정보를 전달하는지 나타낸다. BOUNDARY는 그 과정이 외부와 상호작용하며 기록 가능한 차이를 남기는 자리다.

SOURCE를 물질 창고로만 이해하면 안 된다. 그것은 아직 질량과 전하와 위치가 모두 확정된 입자의 모음이 아니다. 구현에 필요한 가능성과 자유도의 원천이다. 반대로 BOUNDARY는 우주의 물리적 끝만을 뜻하지 않는다. 한 체계가 다른 체계에 결과를 기록하는 모든 유효 인터페이스를 포함한다.

RELATION은 두 층을 잇는 단순한 선이 아니다. 대칭, 위상, 결합, 선택규칙, 보존법칙, 전달커널이 모두 여기에 속한다. 어떤 원천 상태가 같은지 다른지를 가르고, 함께 실현될 수 있는 조합과 금지되는 조합을 정한다.

_Ω = (SOURCE, RELATION, BOUNDARY)_ (2.8)

이 세 항은 다양한 우주를 기술하는 범용 뼈대가 된다. SOURCE의 종류, RELATION의 대칭과 결합, BOUNDARY의 기록 조건이 달라지면 서로 다른 우주 인스턴스를 만들 수 있다. 우리 우주는 그 가운데 관측된 하나의 설정이다.

_U\_i = E(Ξ\_i, R\_i, B\_i; θ\_i)_ (2.9)

### SOURCE는 모든 답을 직접 보관하지 않는다

정보 원장은 질문 X마다 최초 소유자, 최소 입력, 실행규칙, 실현계기, 기록형식, 상태등급과 정밀도를 함께 적는다. 답을 숫자 하나로만 저장하지 않고 그 숫자가 어디에서 왔는지까지 보존하는 것이다.

P(X)=(owner, payload, execution map, trigger, record, status, precision)

여기서 owner는 독립 정보를 처음 가진 층이다. 법칙은 LAW HEADER, 우주별 초기관계와 전역 위상은 SOURCE, 입자 표현 규칙은 phenotype grammar, 현재 상태의 진화는 execution engine, 특정 관측 기록은 renderer와 event instrument가 소유할 수 있다. 같은 정보가 여러 층에 반복 저장된다면 최소계산 원리에 어긋난다.

따라서 SOURCE의 1차원 점은 세 차원 공간에 놓인 작은 물리적 점이 아니라 관계형 입력의 주소다. 보이는 공간의 세 방향은 WRRA 안의 차원필터가 관계를 표현공간으로 변환한 구조적 출력이다. 공간의 전역 연결방식인 위상, 초기 곡률척도와 경계자료가 동역학만으로 정해지지 않는다면 그 부분은 우주 인스턴스의 조건부 INPUT으로 남는다.

초기에는 이 삼분법만으로 충분해 보였다. 그러나 물리적 대상이 나타나는 순간 문제가 생겼다. 원천의 가능성이 경계 기록으로 바뀌는 중간 과정이 한 단어에 너무 많이 눌려 있었다. 관계가 있다는 사실만으로 질량·전하·스핀·위치가 하나의 대상으로 공동 실현되지는 않았다.

이 누락은 뒤에서 RENDERER라는 이름을 얻게 된다. 하지만 그 전에 필터의 정적 구조를 동역학으로 만들고, 여러 내부 채널을 하나의 전달 작용 아래 묶는 작업이 필요했다.

### 관련 연구

**29. The Zeta Null State: Scalar Zeros, Nonzero Internal States, and the Observability Paradox — The Wonsik–Jeongin Null-State System (WJNS)** [10.5281/zenodo.22012524](https://doi.org/10.5281/zenodo.22012524)

**35. The Hypothesis of Geometric Unification of Gravity and Electromagnetism** [10.5281/zenodo.22042522](https://doi.org/10.5281/zenodo.22042522) 〔부록 D ‘메트릭’ 참조〕

**36. The Hypothesis of Geometric Unification of Gravity and Electromagnetism** [10.5281/zenodo.22049218](https://doi.org/10.5281/zenodo.22049218)

**38. Common-Carrier Unification Without a Grand Unified Gauge Field** [10.5281/zenodo.22052565](https://doi.org/10.5281/zenodo.22052565)

## 14장 필터에서 Hamiltonian으로

필터가 무엇을 통과시키는지 말해준다면 Hamiltonian은 통과한 상태가 어떻게 변하는지 말해준다. 두 층을 연결하지 않으면 차원필터는 분류기나 투영기에는 머물 수 있어도 에너지, 안정성, 전이와 산란을 가진 물리모형이 되기 어렵다.

연구에서는 필터 매개변수 θ에 따라 진공 후보 V₀(θ), 유효 Hamiltonian H\_B(θ), 그리고 분해능 E에서의 Green 함수 G(E,θ)를 연결하는 다리를 구상했다. 이 세 항은 선택된 부분공간, 그 위의 동역학, 외부 자극에 대한 응답을 차례로 맡는다.

_F(θ) → V₀(θ) → H\_B(θ) → G(E,θ)_ (2.10)

V₀(θ)는 가능한 진공 가운데 어떤 배경이 인스턴스의 기준이 되는지를 기록한다. H\_B(θ)는 그 배경 위에서 허용된 상태의 시간발전과 에너지 구조를 정한다. G(E,θ)는 주어진 에너지에서 무엇이 전파되고 어디에 pole이나 공명이 나타나는지를 보여준다.

_G(E,θ) = \[E + i0 − H\_B(θ)]⁻¹_ (2.11)

이 다리는 관측상수의 위치도 정리한다. 어떤 값은 구조가 강제하고, 어떤 값은 진공과 경계조건을 지정하는 보정 입력이며, 어떤 값은 그 입력을 고정한 뒤 계산되는 출력이다. 알려진 상수를 보정에 쓰는 것은 당연하지만, 보정값을 예측으로 다시 세지 않는 것이 중요하다.

표준모형도 모든 매개변수를 관측 없이 수치 예측하는 이론은 아니다. 대칭과 장의 내용, 상호작용의 형식을 강하게 제한하지만 질량, 혼합, 결합의 여러 수치는 실험에서 정해진다. 새 구조의 가치는 입력을 숨기는 데 있지 않고, 입력 후 어떤 관계가 강제되고 어떤 새 관측량이 독립적으로 남는지에 있다.

현재 이 다리는 설계 원리와 부분 계산의 단계에 있다. 완전한 작용, 재규격화, 단위성, 인과성과 표준모형 정밀자료를 동시에 닫았다고 주장할 수 없다. 그래서 제2부는 완성이 아니라 WRRA가 해결해야 할 기술적 문턱을 명시한다.

### 관련 연구

**41. An Effective Microscopic Completion of Common-Carrier Unification** [10.5281/zenodo.22055305](https://doi.org/10.5281/zenodo.22055305)

**42. The Common Transport Operator and the Minimal Origin of Chiral Matter** [10.5281/zenodo.22056516](https://doi.org/10.5281/zenodo.22056516) 〔부록 D ‘키랄성’ 참조〕

**46. Retarded Linear Response of a Self-Consistent Bessel Common Carrier** [10.5281/zenodo.22062921](https://doi.org/10.5281/zenodo.22062921)

## 15장 공통전달자와 15채널

다음 문제는 내부 자유도였다. 한 세대의 카이럴 물질을 기술하려면 서로 다른 전하와 표현을 가진 여러 방향이 필요하다. 연구에서는 15개의 채널을 별개의 세계로 흩어놓기보다 하나의 공통 연속체가 모두를 운반하는 구조를 탐색했다.

공통전달자 D\_C는 15방향 전체를 같은 운송 법칙 아래 두려는 장치다. 채널은 서로 다른 내부 표지를 가질 수 있지만 국소 전달, 운동학, 경계 기록은 공통 골격을 공유한다. 이것은 최소계산의 재사용 원리를 입자 내용에 적용한 것이다.

_D\_C : ⊕ᵢ₌₁¹⁵ H\_i → ⊕ᵢ₌₁¹⁵ H\_i_ (2.12)

초기의 민주적 rank-one 결합은 한 밝은 조합만 전달하고 나머지 14방향을 어둡게 남기는 문제가 있었다. 대칭적인 모양이 아름답다고 해서 충분한 물리적 rank가 자동으로 생기지는 않았다. 이 실패는 폐쇄해야 할 반례로 기록되었다.

_rank(D\_C│band) = 15_ (2.13)

보수 방향은 공통전달자를 버리는 것이 아니라 rank를 여는 결합을 추가하는 것이었다. 한 연속체가 전체 band rank를 지니면서도 채널별 전하와 선택규칙을 보존해야 한다. 공통성과 구별 가능성을 동시에 만족해야 한다.

직렬 rotor 구상도 여기서 나왔다. 이것은 채널을 하나씩 기계적으로 켜는 순차 스위치가 아니라, 자율적으로 회전하는 rank-one port가 위상 부호화를 통해 전체 채널과 관계하는 구조다. 시간순 목록이 아니라 공통 운송 위의 phase-coded seriality다.

_P(φ) = |v(φ)⟩⟨v(φ)|, rank P(φ)=1_ (2.14)

15채널은 최종 입자질량과 혼합을 모두 설명했다는 뜻이 아니다. 한 세대 카이럴 carrier의 후보 경계기록이며, 세대 복제·Yukawa·쿼크 혼합·강결합 동역학과 질량의 상류 생성법은 별도 층으로 남는다. 다만 30장에서는 관측된 제1세대 값에서 낮은 정수 양자관계를 찾아 동결하고, 아직 직접 측정되지 않은 중성미자 절대질량 후보를 제시한다. 이는 독립적 상류 유도가 아니라 검증을 기다리는 현상론적 예측이다.

### 관련 연구

**38. Common-Carrier Unification Without a Grand Unified Gauge Field** [10.5281/zenodo.22052565](https://doi.org/10.5281/zenodo.22052565)

**42. The Common Transport Operator and the Minimal Origin of Chiral Matter** [10.5281/zenodo.22056516](https://doi.org/10.5281/zenodo.22056516)

**45. A Minimal Causal Common Carrier for Chiral Matter Creation and Spectral Locking** [10.5281/zenodo.22058494](https://doi.org/10.5281/zenodo.22058494)

**48. An Isotropic Spatial Gap for a Fifteen-Channel Common Carrier** [10.5281/zenodo.22063296](https://doi.org/10.5281/zenodo.22063296)

**49. Autonomous Rank Opening from a Fifteen-Channel Bessel Determinant** [10.5281/zenodo.22063551](https://doi.org/10.5281/zenodo.22063551)

**56. Filter-Restored Revision of the Fifteen-Channel Common-Carrier Model** [10.5281/zenodo.22067895](https://doi.org/10.5281/zenodo.22067895)

**57. Minimum-Computational Filter-Spectral Revision of the Fifteen-Channel Common-Carrier Model** [10.5281/zenodo.22068573](https://doi.org/10.5281/zenodo.22068573)

**58. Ground-Subtracted Lossless-Angle Completion of the Fifteen-Channel Common-Carrier Model** [10.5281/zenodo.22069630](https://doi.org/10.5281/zenodo.22069630)

## 16장 Hardware–Firmware–Software–Execution

복잡한 물리모형이 흔들리는 이유 중 하나는 서로 다른 설명 층의 책임을 섞기 때문이다. WRRA 계보에서는 이를 Hardware, Firmware, Software, Execution의 네 층으로 나눈다. 컴퓨터가 우주 밖에 있다는 뜻이 아니라 구조적 소유권을 분리하는 비유다.

Hardware는 표현과 전하비, 15채널, 공통 운송처럼 무엇이 존재하고 어떤 방향이 연결 가능한지를 맡는다. 이 층이 바뀌면 입자 내용과 허용 표현 자체가 바뀐다.

Firmware는 스펙트럼 가중치, 운동항의 계량, pole의 활성화, matching과 진공 선택을 맡는다. 같은 Hardware라도 어떤 모드가 저에너지에서 보이고 어떤 결합이 유효한지는 이 층에 달려 있다.

Software는 Yukawa 구조, 세대, 혼합각과 CP 위상처럼 물질의 구체적 패턴을 맡는다. 관측된 질량과 혼합을 단순히 표기만 바꿔 이 층에 옮겼다면 재표현일 뿐이다. 새로운 이론적 성과가 되려면 독립 입력을 줄이거나 아직 쓰지 않은 관계를 계산해야 한다.

_M\_Y = Y(Hardware, Firmware; θ\_software)_ (2.15)

Execution은 renormalization-group 흐름, threshold, pole mass처럼 이 구조를 실제 관측 스케일에 맞추는 계산이다. 양자적 실현 뒤 관측치에 맞춘다고 말할 때도 단순 숫자 맞추기와 물리적 실행을 구별해야 한다. 보정용 자료와 사후검증 자료를 나누는 이유다.

_O\_obs(μ) = RG\_μ ∘ Threshold ∘ Pole\[M\_Y]_ (2.16)

이 계층은 연구 실패를 숨기지 않고 위치시킨다. Hardware가 맞아도 Software가 열려 있을 수 있고, tree level 관계가 있어도 Execution에서 깨질 수 있다. 반대로 관측값을 잘 재현했다고 Hardware 원리가 증명되는 것도 아니다.

### 관련 연구

**50. From Autonomous Rank Opening to Matter Production** [10.5281/zenodo.22063716](https://doi.org/10.5281/zenodo.22063716)

**52. Energy-Information Compatibility and Dynamic Boundary Unlocking in a Fifteen-Channel Common Carrier** [10.5281/zenodo.22065409](https://doi.org/10.5281/zenodo.22065409)

**53. Spectral-Owner Matching and Graded Boundary Release in a Fifteen-Channel Common Carrier** [10.5281/zenodo.22066433](https://doi.org/10.5281/zenodo.22066433)

**54. Autonomous Spectral Settlement after Fifteen-Channel Rank Opening** [10.5281/zenodo.22067588](https://doi.org/10.5281/zenodo.22067588)

## 17장 왜 renderer가 필요한가

차원필터, Hamiltonian, 공통전달자와 계층 구분을 거치자 마지막 누락이 선명해졌다. 질량은 질량 연산자에서, 전하는 게이지 표현에서, 스핀은 회전과 로런츠 표현에서, 위치는 국소 대수에서 따로 정의할 수 있다. 그러나 실제 검출기는 이 네 속성을 따로 관측한 뒤 임의로 한 입자에 붙이지 않는다.

물리적 대상은 질량·전하·스핀·위치가 공동으로 귀속되는 하나의 사건 패턴이다. 따라서 대상의 정체성은 여러 속성 목록의 합이 아니라, 같은 국소 관측대수와 같은 번역 작용 아래에서 함께 유지되는 joint phenotype이어야 한다.

_Phenotype = Joint(m, q, s, x │ A\_local, T\_a)_ (2.17)

SOURCE와 BOUNDARY 사이에 renderer가 필요한 이유가 여기에 있다. renderer는 가능성을 그림으로 꾸미는 장식이 아니다. 서로 다른 자유도를 양립 가능한 공동 상태로 묶고, 국소성과 인과성, 대칭과 보존법칙을 지키며, 경계에 재현 가능한 기록을 내보내는 구현 아키텍처다.

이때 phenotype은 생물학적 표현형을 그대로 빌린 말이 아니다. 내부의 원천과 관계가 특정 환경과 경계조건 아래에서 실제 관측 가능한 물리적 대상으로 나타난 결과를 뜻한다. 같은 범용 renderer라도 인스턴스 입력과 진공이 다르면 다른 phenotype 우주가 가능하다.

따라서 WRRA의 기본 흐름은 SOURCE → RENDERER → PHENOTYPE으로 요약된다. RELATION과 BOUNDARY는 renderer의 작동 문법과 기록 인터페이스를 제공한다. 차원필터와 공통전달자는 그 내부 모듈의 후보이며, Hardware에서 Execution까지는 책임 층을 나눈다.

_PHENOTYPE = RENDERER(SOURCE; RELATION, BOUNDARY, θ)_ (2.18)

이 구조는 아직 최종 물리이론의 증명이 아니다. 현재 상태는 개념 아키텍처, 부분적 수학모형, 수치 회귀검사, 실패폐쇄된 경로와 열린 층이 함께 있는 연구 프로그램이다. 하지만 이제 무엇을 묻는 이론인지, 어디까지 닫혔고 무엇이 검증되어야 하는지는 이전보다 분명해졌다.

_SOURCE → RENDERER → PHENOTYPE_ (2.19)

### 관측은 현실의 출력 요청인가

관측 이전에도 내부 상태의 시간 진화는 계속된다. 최소계산 우주론이 절약한다고 보는 것은 존재 그 자체가 아니라, 모든 가능성을 매 순간 하나의 완성된 고전 영상으로 렌더링하는 비용이다. 기록 가능한 상호작용이 생길 때 renderer는 그 시점의 상태와 관측 인터페이스가 허용하는 국소 결과만 현실에 출력한다.

Y\_a(t) = O\_a\[Ψ(t)]

따라서 관측자는 우주 밖에서 현실을 마음대로 창조하는 존재가 아니다. 관측 장치와 환경을 포함한 물리적 상호작용이 출력 조건을 형성하고, 결과는 내부 상태·Born 규칙·보존법칙·관측대수의 결합으로 제한된다. ‘누군가가 볼 때 영상이 출력된다’는 직관은 의식 중심의 마술이 아니라, 기록 가능한 상호작용에서만 공동 현실이 분해된다는 선택적 실현 명제로 번역된다.

SOURCE → READ ORDER → AUTONOMOUS EVOLUTION → SELECTIVE REALIZATION → SHARED RECORD

### 관련 연구

**33. The Hypothesis of Light, Closure, and Rest Mass** [10.5281/zenodo.22041149](https://doi.org/10.5281/zenodo.22041149)

**37. A Tuned Model of Our Universe Based on the Dimensional Filter** [10.5281/zenodo.22051682](https://doi.org/10.5281/zenodo.22051682)

**55. The Universal Minimum-Computation Model and the Non-Special Universe** [10.5281/zenodo.22067717](https://doi.org/10.5281/zenodo.22067717)

## 제2부의 경계와 다음 질문

제2부가 보여준 것은 가능성이 곧 현실이 아니라는 점이다. 차원필터는 가시 부문을 나누고, Hamiltonian은 그 위의 동역학을 주며, 공통전달자는 여러 내부 채널을 하나의 운송 아래 묶는다. 그러나 이 모듈들이 모두 작동해도 관측 가능한 대상의 공동 정체성을 설명해야 한다.

현재 WRRA는 완결된 표준모형 대체물이 아니다. 알려진 상수를 다른 기호로 옮긴 부분은 재표현으로 분류하고, 관측값을 맞춘 부분은 보정으로 표시하며, 입력하지 않은 자료에 대한 독립적 예측만 예측이라 부를 것이다. 유일한 우주의 증명도 목표로 삼지 않는다.

다음 부에서는 SOURCE, RENDERER, PHENOTYPE을 정식으로 정의하고, renderer의 내부 모듈과 양자적 실현, 관측 보정, 반증 가능한 예측의 순서를 세운다. 열린 가능성을 남기는 것은 결함을 숨기는 일이 아니라 연구가 실제로 시작될 좌표를 표시하는 일이다.
