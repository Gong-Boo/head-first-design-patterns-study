## 13. 패턴과 행복하게 살기 - 실전 디자인 패턴

### 디자인 패턴의 정의
- 패턴은 특정 컨텍스트 내에서 주어진 문제의 해결책이다.
- 컨텍스트 : 패턴이 적용되는 상황을 뜻합니다. 반복적으로 일어날 수 있는 상황이어야만 합니다.
- 문제 : 컨텍스트 내에서 이뤄야 하는 목표를 뜻합니다. 여기에는 컨텍스트 내의 제약 조건도 포함됩니다.
- 해결책 : 바로 우리가 찾아내야 하는 것입니다. 제약 조건 속에서 누가 적용해도 목표를 이 수 있는 일반 적인 디자인을 뜻한다.
- "어떤 컨텍스트 내에서 일련의 제약 조건에 의해 영향을 받는 문제가 발생했다면, 그 제약조건 내에서 목적 달성을 위한 해결책이 되는 디자인을 적용하면 된다"

### 새로운 디자인 패턴 만들기
1. 먼저 기존의 패턴을 확실히 파악한다.
2. 지금까지의 경험을 토대로 다시 한번 곰곰이 생각해 보고, 반복적으로 발생하는 문제를 해결할 수 있는 새로운 디자인이 되도록 다음어야 한다.
3. 새로운 패턴을 발견 했다면, 다른 사람들이 직접 적용해 보고 피드백을 제공할 수 있도록 문서로 만들어 보자.
4. 새로운 패턴은 시간이 지남에 따라 점점 나아진다. 피드백을 얻어라

### 디자인 패턴 분류하기
- 대부분의 카탈로그에서는 몇 가지 범주에 맞춰서 디자인 패턴을 분류하고 있다.
- 그중 제일 유명한 방법은 생성, 행동, 구조로라는 3가지 범주로 용도에 따라 나누기이다.

1. 생성 패턴 : 객체 인스턴스를 생성하는 패턴으로, 클라이언트와 그 클라이언트가 생성해야 하는 객체 인스턴스 사이의 연결을 끊어 주는 패턴이다.
2. 행동 패턴 : 클래스와 객체들이 상호작용하는 방법과 역활을 분담하는 방법을 다루는 패턴이다.
3. 구조 패턴 : 클래스와 객체를 더 큰 구조로 만들 수 있게 구상을 사용하는 패턴이다.

- 앞쪽에 보여준 범주와는 별개로 클래스를 다루는 패턴인지, 객체를 다루는 패턴인지 따라 분류하는 법도 있다.

### 패턴으로 생각하기
-까다로운 이론을 아무리 많이 알고 있다고 해도 경험과 연습 없이는 별로 도움이 되질 못한다. 아래는 패턴으로 생각하는데 있어서 도움될 몇가지다.

1. 최대한 단순하게 - 가장 중요한건 최대한 단순한 방법으로 문제를 해결하기다
2. 디자인 패턴은 만병 통치약이 아니다 - 패턴을 사용 할때는 그 패턴이 설계한 디자인에 미칠 영향과 결과를 주의 깊게 되야한다.
3. 패턴이 필요할 때 - 디자인상의 문제에 적합하다는 확신이 든다면 패턴을 도입해야한다.
4. 리팩터링과 패턴 - 리팩터링은 구조개선에 초점이 맞춰져 있다. 패턴을 사용하면 구조가 더 개선될수 있을지 검토해 볼수있는 아주 좋은 기회다.
5. 꼭 필요하지 않은 패턴은 빼버리자. 지금 있는 디자인에서 디장니 패턴을 제거하는 일을 두려워 하지마라
6. 꼭 필요하지 않은 패턴을 미리 적용할 필요 없다.

### 패턴을 대하는 마음가짐
- 초보자들은 언제나 패턴을 사용하려는 경향이 있다.
- 중급자 수준에 오르면 어떤 상황에 패턴이 필요하고 필요하지 않은지를 파악할 수 있다.
- 그랜드 마스터의 경지에 오르면 패턴을 자연스럽게 구사할 수 있다.

### 안티 패턴 섬멸하기
- 안티패턴은 어떤 문제의 나쁜 해결책에 이르는 길을 알려줍니다.
