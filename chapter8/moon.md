## 템플릿 메소드 패턴

### 템플릿 메소드 패턴 알아보기
- 템플릿 메소드는 알고리즘의 각단계를 정의하며, 서브클래스에서 일부 단계를 구현할 수 있도록 유도합니다.

### 템플릿 메소드의 장점 알아보기
- 하나의 클래스에서 작업을 처리하여 알고리즘을 독점한다.
- 서브클래스에서 코드를 재사용할 수 있다.
- 알고리즘이 한 군데에 모여 있으므로 한 부분만 고치면 된다.
- 클래스에 알고리즘 지식이 집중되어 있으며 일부 구현만 서브클래스에 의존한다.

### 탬플릿 메소드 패턴의 정의
- 템플릿 메소드패턴은 알고리즘의 골격을 정의한다. 
- 템플릿 메소드를 사용하면 알고리즘의 일부 단계를 서브클래스에서 구현할 수 있으며, 알고리즘의 구조는 그대로 유지하면서 알고리즘의 특정 단계를 서브클래스에서 재정의할 수도 있다.

### 템플릿 메소드 속 후크 알아보기
- 후크는 추상 클래스에서 선언되지만 기본적인 내용만 구현 되어 있거나 아무 코드도 들어있지 않은 메소드다.
- 이러면 서브 클래스는 다양한 위치에서 알고리즘에 끼어 들수 있다.

### 새로운 디자인 원칙
- 할리우드 원칙 : 먼저 연락하지 마세요 저희가 연락 드리겠습니다.
- 할리우드 원칙을 확용하면 의존성 부패를 방지할수 있다.
- 의존성이 얽혀 복잡하게 꼬여있는 상황을 의존성 부패라고 한다.
- 즉 고수준 구성 요소가 저수준 구성요소에게 "먼저 연락하지 마세요. 제가 연락 드리겠습니다"라고 얘기 하는것과 같다.
