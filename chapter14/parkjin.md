# 기타 패턴

### 브리지 패턴
구현과 더불어 추상화 부분까지 변경해야 한다면 브리지 패턴을 쓰면 된다

활용법
- 여러 플랫폼에서 사용해야 하는 그래픽스와 윈도우 처리 시스템에서 유용하게 쓰인다
- 인터페이스와 실제 구현할 부분을 서울 다른 방식으로 변경해야 할 때 유용하게 쓰인다

장점
- 구현과 인터페이스를 완전히 결합하지 않았기에 구현과 추상화 부분을 분리할 수 있다
- 추상화된 부분과 실제 구현 부분을 독립적으로 확장할 수 있다
- 추상화 부분을 구현한 구상 클래스가 바뀌어도 클라이언트에 영향을 끼치지 않는다

단점
- 디자인이 복잡해진다

### 빌더 패턴
제품을 여러 단계로 나눠서 만들도록 제품 생산 단계를 캡슐화하고 싶다면 빌더 패턴을 사용하면 된다

활용법
- 복합 객체 구조를 구축하는 용도로 많이 쓰인다

장점
- 복합 객체 생성 과정을 캡슐화한다
- 여러 단계와 다양한 절차를 거쳐 객체를 만들 수 있다
- 제품의 내부 구조를 클라이언트로부터 보호할 수 있다
- 클라이언트는 추상 인터페이스만 볼 수 있기에 제품을 구현한 코드를 쉽게 바꿀 수 있다

단점
- 복합 객체 구조를 구축하는 용도로 많이 쓰인다

### 책임 연쇄 패턴
1개의 요청을 2개 이상의 객체에서 처리해야 한다면 책임 연쇄 패턴을 사용하면 된다

활용법
- 윈도우 시스템에서 마우스 클릭과 키보드 이벤트를 처리할 때 흔히 쓰인다

장점
- 요청을 보낸 쪽과 받는 쪽을 분리할 수 있다
- 객체는 사슬의 구조를 몰라도 되고 그 사실에 들어있는 다른 객체의 직접적인 레퍼런스를 가질 필요도 없으므로 객체를 단순하게 만들 수 있다
- 사슬에 들어가는 객체를 바꾸거나 순서를 바꿈으로써 역할을 동적으로 추가하거나 제거할 수 있다

단점
- 요청이 반드시 수행된다는 보장이 없다
- 실행 시에 과정을 살펴보거나 디버깅하기가 힘들다

### 플라이웨이트 패턴
어떤 클래스의 인스턴스 하나로 여러 개의 '가상 인스턴스'를 제공하고 싶다면 플라이웨이트 패턴을 사용하면 된다

활용법
- 어떤 클래스의 인스턴스가 아주 많이 필요하지만 모두 똑같은 방식으로 제어해야 할 때 유용하게 쓰인다

장점
- 실행 시에 객체 인스턴스의 개수를 줄여서 메모리를 절약할 수 있다
- 여러 '가상' 객체의 상태를 한곳에 모아 둘 수 있다

단점
- 이 패턴을 써서 구현해 놓으면 특정 인스턴스만 다른 인스턴스와 다르게 행동하게 할 수 없다

### 인터프리터 패턴
어떤 언어의 인터프리터를 만들 때는 인터프리터 패턴을 사용하면 된다

활용법
- 간단한 언어를 구현할 때 인터프리터 패턴이 유용하게 쓰인다
- 효율보다는 단순하고 간단하게 문법을 만드는 것이 더 중요한 경우에 유용하다
- 스크립트 언어와 프로그래밍 언어에서 모두 쓸 수 있다

장점
- 문법을 클래스로 표현해서 쉽게 언어를 구현할 수 있다
- 문법이 클래스로 표현되므로 언어를 쉽게 변경하거나 확장 할 수 있다
- 클래스 구조에 메소드만 추가하면 프로그램을 해석하는 기본 기능 외에 예쁘게 출력하는 기능이나 더 나은 프로그램 확인 기능 같은 새로운 기능을 추가할 수 있다

단점
- 문법 규칙의 개수가 많아지면 아주 복잡해진다는 단점이 있기에 파서나 컴파일러 생성기를 쓰는 편이 낫다

### 중재자 패턴
서로 연관된 객체 사이의 복잡한 통신과 제어를 한곳으로 집중하고 싶다면 중재자 패턴을 쓰면 된다

활용법
- 서로 연관된 GUI 구성 요소를 관리하는 용도로 많이 쓰인다

장점
- 시스템과 객체를 분리함으로써 재사용성을 획기적으로 향상시킬 수 있다
- 제어 로직을 한 군데 모아놨으므로 관리하기가 수월하다
- 시스템에 들어있는 객체 사이에서 오가는 메시지를 확 줄이고 단순화 할 수 있다

단점
- 디자인을 잘 하지 못하면 중재자 객체가 너무 복잡해질 수 있다

### 메멘토 패턴
객체를 이전의 상태로 복구해야 한다면 메멘토 패턴을 쓰면 된다

활용법
- 메멘토 객체를 써서 상태를 저장한다
- 자바 시스템에서는 시스템의 상태를 저장할 때 직렬화를 사용하는 것이 좋다

장점
- 저장된 상태를 핵심 객테와는 다른 별도의 객체에 보관할 수 있어 안전하다
- 핵심 객체의 데이터를 계속해서 캡슐화된 상태로 유지할 수 있다
- 복구 기능을 구현하기가 쉽다

단점
- 상태를 저장하고 복구하는 데 시간이 오래 걸릴 수 있다는 단점이 있다

### 프로토패턴
어떤 클래스의 인스턴스를 만들 때 자원과 시간이 많이 들거나 복잡하다면 프로토타입 패턴을 쓰면 된다

 활용법
 - 시스템에서 복잡한 클래스 계층구조에 파묻혀 있는 다양한 형식의 개체 인스턴스를 새로 만들어야 할 때 유용하다

장점
- 클라이언트는 새로운 인스턴스를 만드는 과정을 몰라도 된다
- 클라이언트는 구체적인 형식을 몰라도 객체를 생성할 수 있다
- 상황에 따라서 객체를 생성하는 것보다 객체를 복사하는 것이 더 효율적일 수 있다

단점
- 떄때로 객체의 복사본을 만드는 일이 매우 복잡할 수도 있다

### 비지터 패턴
다양한 객체에 새로운 기능을 추가해야 하는데 캡슐화가 별로 중요하지 않다면 비지터 패턴을 쓰면 된다

장점
- 구조를 변경하지 않으면서도 복합 객체 구조에 새로운 기능을 추가할 수 있다
- 비교적 손쉽게 새로운 기능을 추가할 수 있다
- 비지터가 수행하는 기능과 관련된 코드를 한곳에 모아 둘 수 있다

단점
- 비지터를 사용하면 복합 클래스의 캡슐화가 깨진다
- 컬렉션 내의 모든 항목에 접근하는 트래버서가 있으므로 복합 구조를 변경하기가 더 어렵다
