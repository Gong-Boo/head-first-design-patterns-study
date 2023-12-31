# 반복자 패턴과 컴포지트 패턴
- 둘 중 한 명이 양보하지 않는 이상 종업원을 구현하는 일이 상당히 불편해 지고, 코드 관리와 확장이 힘들어 집니다.
- 인터페이스가 같아지면 종업워 코드에서 구상 객체의 레퍼런스를 거의 안 써도 되고, 각 메뉴에 있는 항목을 전부 찾으려고 순환문을 여러 개 쓸 필요도 없습니다.
- 바귀는 부분을 캡슐화하라
- 그냥 반복자로 메뉴에 들어있는 항목 하나하나에 접근할 수만 있으면 됩니다.
- ArrayList에 반복자를 리턴하는 iterator() 메소드도 있습니다.
- 배열에 iterator() 메소드가 없기도 하고, 배열 반복자를 만드는 방법 자체가 아예 없으니까요.
- 반복자 패턴은 컬랙션의 구현 방법을 노출하지 않으면서 집합체 내의 모든 항목에 접근하는 방법을 제공합니다.
- 각 항목에 일일이 접근할 수 있게 해 주는 기능을 집합체가 아닌 반복자 객체가 책임진다는 장점도 있습니다.
- 컴포지트 패턴으로 객체를 트리구조로 구성해서 부분-전체 계층구조를 구현합니다.
- 컴포지트 패턴을 사용하면 클라이언트에서 개별 객체와 복합 객체를 똑같은 방법으로 다룰 수 있습니다.
- 잎과 복합 노드 모두에서 쓰이는 인터페이스 역할을 한다는 저을 꼭 기억해 둡시다.
- 단일 역할 원칙을 깨는 대신 투명성을 확보하는 패턴이라고 할 수 있습니다.
- 상황에 따라 원칙을 적절하게 사용해야 함을 보여 주는 대표 사례라고 할 수 있습니다.
