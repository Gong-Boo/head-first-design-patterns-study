## 싱글턴 패턴

### 싱글턴 패턴의 정의
- 싱글턴 패턴은 클래스 인스턴스를 하나만 만들고, 그 인스턴스로의 전역 접근을 제공합니다.
- 싱글턴 패턴을 실제로 적용할 때는 클래스에서 하나뿐인 인스턴스를 관리하도록 만들어야 합니다.
- 어디서든 그 인스턴스에 전근 할수 있도록 전역 접근 지점을 제공합니다.

### 멀티 스레딩 문제
- 싱글턴 객체를 멀티 스레딩 할 경우 동시에 getInstance에 접근하여 객체가 2개가 될수있다.
- getInstance함수는 sychronized를 통해 동시 실행을 막아준다.

### 더 효율적으로 멀티스레딩 문제 해결하기
- getInstance() 메소드를 동기화 하면 적지 않은 대가를 치뤄야 한다 다른 방법은 없을까?
- 1. getInstance()의 속도가 중요하지 않는다면 그냥둔다.
  2. 인스턴스가 필요할 때는 생성하지 말고 처음부터 만들어 둔다.
  3. DCL을 써서 getInstance()에서 동기화 되는 부분을 줄인다.

### 싱글턴 Q&A
- 모든 메소드와 변수가 static이면 결과적으로 싱글턴 패턴과 같지 않은가? - 복잡한 초기화가 필요 없는 경우 가능하다. 하지만 여러 클래스가 얽혀 있다면 지저분해진다.
- 클래스 로더와 관련된 문제는 없는가? - 클래스 로더가 여러개라면 조심해야 한다. 물론 클래스 로더를 직접 지정하면 문제없다.
- 리플렉션, 직렬화, 역질렬화 문제도 있지 않은가? - 문제가 된다. 위에 3개 기능을 사용하는 고급 자바 사용자라면 그점을 염두에 둬야한다.

