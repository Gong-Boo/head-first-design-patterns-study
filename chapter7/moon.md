## 어탭터 패턴과 퍼사드 패턴

### 어댑터 살펴보기
- 우리 주변에 있는 어댑터를 살펴보면 객체지향 어댑터가 무엇인지 쉽게 이해할수 있다.
- 한국에서 사용하던 휴대전화 충전기를 영국에서도 사용하려면 플러그 모양을 바꿔주는 어댑터가 필요하다.
- 객체지향 어댑터도 일상생활에서 쓰이는 어댑터와 똑같은 역활을 말합니다.
- 어떤 인터페이스든 클라이언트에서 요구하는 형태로 적용시키는 역활을 한다.

### 객체지향 어댑터 알아보기
- 기존시스템에 새로운 업체의 시스템을 사용해야 하는데 서로 인터페이스가 다르다고 가정해보자.
- 그런데 기존 코드를 바꿔서 이를 해결할수 없다.
- 새로운 업체에서 사용하는 인터페이스를 기존에 사용하던 인터페이스에 적응시켜주는 클래스를 만들면 된다.
- 어댑터는 클라이언트로부터 요청을 받아서 새로운 업체에서 제공하는 클래스를 클라이언트가 받아들일 수 있는 형태의 요청으로 변환해준다.

### 클라이언트에서 어탭터를 사용하는 방법
1. 클라이언트에서 타깃 인터페이스로 메소드를 호출해서 어댑터에 요청을 보낸다.
2. 어댑터는 어댑터 인터페이스로 그 용청을 어댑터에 관한 메소드 호출로 변환한다.
3. 클라이언트는 호출 결과를 받긴 하지만 중간에 어댑터가 있다는 사실을 모른다.

### 어탭터 패턴의 정의
- 어댑터 패턴은 특정 클래스 인터페이스를 클라이언트에서 요구하는 다른 인터페이스로 변환한다.
- 인터페이스가 호환되지 않아 같이 쓸 수 없었던 클래스를 사용할 수 있게 도와준다.

### 퍼사드 패턴 정의
- 퍼사드 패턴은 서브시스템에 있는 일련의 인터페이스를 통합 인터페이스로 묶어 줍니다. 또한 고수준 인터페이스도 정의하므로 서브시스템을 더 편리하게 사용할수 있다.

### 최소 지식 원칙
- 디자인 원칙 : 진짜 절친에게만 이야기 해야한다.
- 최소 지식 원칙에 따르면 객체 사이의 상호작용은 될 수 있으며 아주 가까운 친구 사이에서만 허용하는 편이 좋다.
