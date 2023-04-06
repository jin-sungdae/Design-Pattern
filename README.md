##디자인 패턴
- 자주 사용하는 설계 패턴을 정형화 해서 이를 유형별로 가장 최적의 방법으로 개발을 할 수 있도록 정해둔 설계
- 알고리즘과 유사하지만, 명확하게 정답이 있는 형태는 아니며, 프로젝트의 상황에 맞추어 적용 가능하다.
## Gof 디자인 패턴
- 소프트웨어를 설계할 때는 기존에 경험이 매우 중요하다. 그러나 모든 사람들이 다양한 경험을 가지고 있을 수는 없다.
- 이러한 지식을 공유하기 위해서 나온 것이 ``GOF(Gan of Four)``의 디자인 패턴이다. 객체지향 개념에 따른 설계중 재사용할 경우 유용한 설계를 디자인 패턴으로 정리 해둔 것이다.
Gof의 디자인 패턴은 총 23개 이며, 이를 잘 이해하고 활용한다면, 경험이 부족하더라도 좋은 소프트웨어 설계가 가능하다.

## 디자인 패턴의 장점
- 개발자(설계자) 간의 원활한 소통
- 소프트웨어 구조 파악 용이
- 재사용을 통한 개발 시간 단축
- 설계 변경 요청에 대한 유연한 대처
## 디자인 패턴의 단점
- 객체지향 설계 / 구현
- 초기 투자 비용 부담

## Singleton pattern

- Singleton 패턴은 어떠한 클래스(객체) 가 유일하게 1개만 존재 할 때 사용한다.
- 이를 주로 사용하는 곳은 서로 자원을 공유 할 때 사용하는데, 실물 세계에서는 프린터가 해당되며, 실제 프로그래밍에서는 TCP Socket통신에서 서버와 연결된 connect 객체에 주로 사용한다.

![](https://velog.velcdn.com/images/sjin/post/1a7163c7-e148-4eeb-a8b6-b95cab76842a/image.png)

---
## Adapter pattern
- Adapter는 실생활에서는 100v를 220v로 변경해주거나, 그 반대로 해주는 흔히 돼지코 라고 불리는 변환기를 예로 들 수 있다.
- 호환성이 없는 기존 클래스의 인터페이스를 변환하여 재사용 할 수 있도록 한다.
- SOLID중에서 개방폐쇄 원칙(OCP)를 따른다.

![](https://velog.velcdn.com/images/sjin/post/f248af30-6b17-4f4f-ba68-bf31315f27cb/image.png)

---
## Proxy Pattern
- Proxy는 대리인 이라는 뜻으로써, 뭔가를 대신해서 처리하는 것
- Proxy Class를 통해서 대신 전달하는 형태로 설계되며, 실제 CLient는 Proxy로 부터 결과를 받는다.
- Cache의 기능으로도 활용이 가능 하다.
- SOLID중에서 개방폐쇄 원칙 (OCP)과 의존 역전 원칙 (DIP)를 따른다.

![](https://velog.velcdn.com/images/sjin/post/01328965-95f9-421b-ba85-118e7cc39e3e/image.png)

---
## Decorator Pattern
- 데코레이터 패턴은 기존 뼈대 (클래스)는 유지하되, 이후 필요한 형태로 꾸밀 때 사용한다. 확장이 필요한 경우 상속의 대안으로도 활용한다. 
- SOLID중에서 개방폐쇄 원칙(OCP)과 의존 역전 원칙(DIP)를 따른다.

![](https://velog.velcdn.com/images/sjin/post/227bc6be-86c1-4f4c-b840-73fc3b28c0a4/image.png)

---

## Observer Pattern
- 관찰자 패턴은 변화가 일어 났을 때, 미리 등록된 다른 클래스에 통보해주는 패턴을 구현한 것이다.
- 많이 보이는 곳은 event listener에서 해당 패턴을 사용 하고 있다.

![](https://velog.velcdn.com/images/sjin/post/d3c99deb-40c8-4902-b5a3-a706c64b4b3c/image.png)

---

## Fascade Pattern
- Facade는 건물의 앞쪽 정면 이라는 뜻을 가진다.
- 여러 개의 객체와 실제 사용하는 서브 객체의 사이에 복잡한 의존 관계가 있을 때, 중간에 facade 라는 객체를 두고, 여기서 제공하는 interface만을 활용하여 기능을 사용하는 방식이다.
- Facade는 자신이 가지고 있는 각 클래스의 기능을 명확히 알아야 한다.

![](https://velog.velcdn.com/images/sjin/post/7283d0cb-f1ac-4221-9149-4b3e976fbcdd/image.png)

---

## Strategy Pattern
- 전략 패턴으로 불리며, 객체지향의 꽃이다.
- 유사한 행위들을 캡슐화 하여, 객체의 행위를 바꾸고 싶은 경우 직접 변경하는 것이 아닌 전략만 변경 하여, 유연하게 확장하는 패턴
- SOLID 중에서 개방폐쇄 원칙 (OCP)과 의존 역전 원칙 (DIP)를 따른다.

![](https://velog.velcdn.com/images/sjin/post/a90b5410-ff1c-4fc0-99a5-bf62889bfef2/image.png)

---