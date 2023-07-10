## 팩토리 패턴

### new 연산자가 눈에 띈다면 구상 이라는 용어를 떠올려라
- new를 사용하면 구상 클래스의 인스턴스가 만들어진다.
- 당연히 인터페이스가 아닌 특정 구현을 사용하는 거다.
- 구상 클래스를 바탕으로 코딩하면 나중에 코드를 수정해야 할 가능성이 커지고, 유연성이 떨어진다.

### new에 어떤 문제가 있는 걸까?
- new에는 문제가 없다. 진짜 문제는 변화 이다.
- 인터페이스에 맞춰서 코딩하면 여러 변화에 대응할수 있다. 다 다형성 덕분이다.
- 반대로 구상 클래스를 많이 사용하면 변경에 닫힌 코드가 된다.
- 새로운 구상 형식을 써서 확장 해야 할 때는 어떻게 해서든 다시 열 수 있게 만들어야 한다.

### 간단한 팩토리의 정의 
- 간단한 팩토리는 디자인 패턴보다는 프로그래밍에 자주 쓰이는 관용구에 가깝다.
- 팩토리는 정확하게 팩토리 패턴은 아니다.
- 팩토리 메소드는 객채 생성을 서브클래스에 캡슐화 할 수 있다. 그러면 슈퍼 클래스에 있는 클라이언트 코드와 서브클래스에 있는 객체 생성 코드 분리 가능.

### 팩토리 메소드 패턴 살펴보기
- 모든 팩토리 패턴은 객체 생성을 캡슐화 한다.
- 팩토리 메소드 패턴은 서브클래스에서 어떤 클래스를 만들지 결정함으로써 객체 생성을 캡슐화 한다.

### 팩토리 메소드 패턴의 정의
- 팩토리 메소드 패턴에서는 객체를 생성할때 필요한 인터페이스를 만든다. 어떤 클래스의 인스턴스를 맘ㄴ들지는 서브클래스에서 결정한다.
- 팩토리 메소드 패턴을 사용하면 클래스 인스턴스 만드는 일을 서브클래스에 맡기게 된다.

### 의존성 뒤집기 원칙
- 추상화 된것에 의존하게 만들고 구상 클래스에 의존하지 않게 만든다.
- 고수준 구성 요소가 저수준 구성 요소에 의존하면 안되며, 항상 추상화에 의존하게 만들어야 한다.

### 의존성 뒤집기 원칙을 지키는 방법
- 변수에 구상 클래스의 레퍼런스를 저장하지 않는다.
- 구상 클래스에서 유도된 클래스를 만들지 않는다.
- 베이스 클래스에 이미 구현되어 있는 메소드를 오버라이드 하지 않는다.
- 이 가이드 라인은 항상 지켜야하는 규칙이 아니라 지향해야 할 바를 알려줄 뿐이다.

### 추상 팩토리 패턴의 정의
- 추상 팩토리 패턴은 구상 클래스에 의존하지 않고도 서로 연관되거나 의존적인 객체로 이루어진 제품군을 생산하는 인터페이스를 제공한다.
- 구상클래스는 서브클래스에서 만든다.