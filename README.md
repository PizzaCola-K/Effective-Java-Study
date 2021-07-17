# PostSquad2021 - Effective Java Study 운영 
- 버전 : 210703

##  목차

1. 진행현황 : [위치로 이동](https://github.com/d-h-k/Effective-Java-Study/blob/main/README.md#%EC%8A%A4%ED%84%B0%EB%94%94-%EC%A7%84%ED%96%89%ED%98%84%ED%99%A9)
2. 운영방법 : [위치로 이동](https://github.com/d-h-k/Effective-Java-Study/blob/main/README.md#effective-java-study-%EC%9A%B4%EC%98%81%EB%B0%A9%EB%B2%95)
3. 진행방식 : [위치로 이동](https://github.com/d-h-k/Effective-Java-Study/blob/main/README.md#-%EC%8A%A4%ED%84%B0%EB%94%94-%EC%A7%84%ED%96%89%EB%B0%A9%EC%8B%9D)
4. Q&A : [위치로 이동](https://github.com/d-h-k/Effective-Java-Study/blob/main/README.md#qa)

  
<br><hr><br>

## 스터디 진행현황

<br>

### 2장. 객체 생성과 파괴

| 아이템   | 발표준비 | 이슈 바로가기 |
| ------------------------------- | -------- | -------- |
| 아이템 1. 생성자 대신 정적 팩터리 메서드를 고려하라          |   어거스트, 동       |  |
| 아이템 2. 생성자에 매개변수가 많다면 빌더를 고려하라         |   새리, 케이       |  |
| 아이템 3. private 생성자나 열거 타입으로 싱글턴임을 보증하라 |   노을, 연, 파이로       |  |
| 아이템 4. 인스턴스화를 막으려거든 private 생성자를 사용하라  |   케이, 노을       | [item4](https://github.com/d-h-k/Effective-Java-Study/issues/4) |
| 아이템 5. 자원을 직접 명시하지 말고 의존 객체 주입을 사용하라 |    동, 노을, 파이로      | [item5](https://github.com/d-h-k/Effective-Java-Study/issues/5) |
| 아이템 6. 불필요한 객체 생성을 피하라                        |   어거스트, 동      | [item6](https://github.com/d-h-k/Effective-Java-Study/issues/6) |
| 아이템 7. 다 쓴 객체 참조를 해제하라                         |    동 ,케이  | [item7]() |
| 아이템 8. finalizer와 cleaner 사용을 피하라                  |  노을,파이로     | [item8]() |
| 아이템 9. try-finally보다는 try-with-resources를 사용하라    |   파이로, 어거스트   | [item9]() |

<br>

### 3장. 모든 객체의 공통 메서드

| 아이템                                                   | 발표준비 |
| -------------------------------------------------------- | -------- |
| 아이템 10. equals는 일반 규약을 지켜 재정의하라          |          |
| 아이템 11. equals를 재정의하려거든 hashCode도 재정의하라 |          |
| 아이템 12. toString을 항상 재정의하라                    |          |
| 아이템 13. clone 재정의는 주의해서 진행하라              |          |
| 아이템 14. Comparable을 구현할지 고려하라                |          |

<br>

### 4장. 클래스와 인터페이스
| 아이템 | 발표준비  |
| ----------------------------------- | ---- |
| 아이템 15. 클래스와 멤버의 접근 권한을 최소화하라            |       |
| 아이템 16. public 클래스에서는 public 필드가 아닌 접근자 메서드를 사용하라 |      |
| 아이템 17. 변경 가능성을 최소화하라                          |      |
| 아이템 18. 상속보다는 컴포지션을 사용하라                    ||
| 아이템 19. 상속을 고려해 설계하고 문서화하라. 그러지 않았다면 상속을 금지하라. |      |
| 아이템 20. 추상 클래스보다는 인터페이스를 우선하라           |      |      
| 아이템 21. 인터페이스는 구현하는 쪽을 생각해 설계하라        |      |
| 아이템 22. 인터페이스는 타입을 정의하는 용도로만 사용하라    |      |
| 아이템 23. 태그 달린 클래스보다는 클래스 계층구조를 활용하라 |      |
| 아이템 24. 멤버 클래스는 되도록 static으로 만들라            |      |
| 아이템 25. 톱레벨 클래스는 한 파일에 하나만 담으라           |      |

<br>

### 5장. 제네릭      
| 아이템 |  발표     |
| ----------------------- | ---- |
| 아이템 26. 로 타입은 사용하지 말라                           |      |      
| 아이템 27. 비검사 경고를 제거하라                            |      |      
| 아이템 28. 배열보다는 리스트를 사용하라                      |      |      
| 아이템 29. 이왕이면 제네릭 타입으로 만들라                   |      |      
| 아이템 30. 이왕이면 제네릭 메서드로 만들라                   |      |      
| 아이템 31. 한정적 와일드카드를 사용해 API 유연성을 높이라    |      |      
| 아이템 32. 제네릭과 가변인수를 함께 쓸 때는 신중하라         |      |      
| 아이템 33. 타입 안전 이종 컨테이너를 고려하라                |      |      

<br>

### 6장. 열거 타입과 애너테이션
| 아이템 | 발표준비 |
| ----------------------------------- | ---- |
| 아이템 34. int 상수 대신 열거 타입을 사용하라                |      |      |      |
| 아이템 35. ordinal 메서드 대신 인스턴스 필드를 사용하라      |      |      |      |
| 아이템 36. 비트 필드 대신 EnumSet을 사용하라                 |      |      |      |
| 아이템 37. ordinal 인덱싱 대신 EnumMap을 사용하라            |      |      |      |
| 아이템 38. 확장할 수 있는 열거 타입이 필요하면 인터페이스를 사용하라 |      |      |      |
| 아이템 39. 명명 패턴보다 애너테이션을 사용하라               |      |      |      |
| 아이템 40. @Override 애너테이션을 일관되게 사용하라          |      |      |      |
| 아이템 41. 정의하려는 것이 타입이라면 마커 인터페이스를 사용하라 |      |      |      |

<br><hr><br>

## Effective Java Study 운영방법 
- 스터디가 진행되는 기간, 인원, 스터디 준비에 필요한 힌트들(참고한 리포)

### 스터디 진행기간

- 일정 : 2021. 07. 03(토) ~ 2021. 10. 23(토) - 대략 4개월
  - 9.25일 추석 휴무
- 매주 토요일 10시에 zoom으로 진행합니다.
- 🙂 첫째주는 OT겸 워밍업으로, 자료준비 없이 책만 간단히 읽어오시고, 이전 기수 자료를 참고해도 됩니다! (코쿼 프로젝트로 쌓인 피로도를 고려해서
- 마지막 주에는 전체 회고(+점심회식?) 진행
  - ( 코로나 상황 안정 && 오프라인 스터디 원하시는 분들 )
- 사용가능한 공간
  - 카페 (잠실할리스 외..)
  - 코드스쿼드
  - 대여스터디룸

<br>

### 스터디 인원 구성 :

  - Best case :  5명 (목표),
  - 최대 10명, 최소 3명 시작
  - 참여 확정 : **어거스트, 동, 새리, 케이, 노을, 연, 파이로 > 7명(2021.07.02 기준)**

<br>

### 스터디 준비의 힌트

- 책 정보
  - 책 정보 링크 : [교보문고 링크](귀찮아욬ㅋ...) ,  [알라딘 링크](https://www.aladin.co.kr/shop/wproduct.aspx?ItemId=171196410)
  - 이펙티브자바 공식 Github : [이펙티브자바 공식 Github 링크](https://github.com/WegraLee/effective-java-3e-source-code)
  - [이펙티브자바 3판 번역 용어 설명](https://docs.google.com/document/d/1Nw-_FJKre9x7Uy6DZ0NuAFyYUCjBPCpINxqrP0JFuXk/edit)
- 다들 각자의 인생이 있어서 스터디가 어떤주는 지치고 힘들수 있고, 어떤주는 특별한 일정때문이고, 또 어떨때는 아무이유없이 쉬고 싶을수 있어요..!! 그래서 참고할 수 있는 다른 이펙티브 자바 스터디들의 링크를 준비해봤어요 어렵고 힘들때 몰래몰래 사용하면 좋습니다 😎
  - **```힌트```**
    - 다른 스터디 레포 : https://github.com/Blog-Posting/book-effective-java
    - 백기선님 이펙티브 자바 : https://github.com/keesun/study/tree/master/effective-java
    - 이전에 다른 스터디 레포 참고 2 :  (코쿼분들)
<br>

### 스터디 개선사항 (마음의 소리)

- 스터디는 다함께 만들어나가는 사람들이 모이는 공동체입니다 그래서..
  - 힘들고 지칠때가 있어요 힘들때는 자신의 감정과 상태를 솔직하게 표현해주세요 😰
  - 스터디 요일/시간/방식 등등... 모든것들에 대하여 건의사항이 있으면 적극적으로 의사표현을 해주세요! 적극반영하겠습니다 😎
- 커뮤니케이션을 위해 카톡방을 사용합니다.
- 스터디에 대한 궁금하신 사항은 Dong에게 개인톡 혹은 카톡방에 보내주시면 됩니다.

<br><hr><br>

## 📜 스터디 진행방식

### 온라인 미팅(발표준비, 사전학습)
- 매주 3(1+2)개의 아이템을 학습합니다
  - 3개의 아이템을 모두 학습하고, 학습결과물을 깃헙레포에 업로드 해주세요
  - 매주 1개의 아이템에 대하여 발표합니다
  - 나머지 2개의 아이템에 대해서는 발표하지 않습니다!(Only 토론) 
- 발표가 모두 끝나면 20분 내외의 회고를 진행합니다.
- 발표와 회고에 대한 내용은 아래를 참고해주세요.

### 아이템 선정

- 매주 Effective Java의 아이템 3개를 진행합니다.
- 차주 발표 아이템 선정은 발표가 끝난 후 사다리 타기를 통해 결정합니다.
- 아이템이 선정 한후 다른 분과 아이템 변경은 가능합니다.
- 대신 꼭 슬랙 채널(이펙티브 자바 스터디)에 발표자 선정 글에 변경 사항을 댓글로 남겨주세요.(아래 예시를 참고해주세요.)
  ```
  아이템 변경
  김자바 15 > 17 
  박디비 17 > 15
  ```

### 아이템별 이슈/학습내용 관리

- 하나의 아이템 마다 하나의 Github Issue가 등록 됩니다.
- 각 아이템들을 공부하다가 이해가 되지 않거나 토론할 내용이 있다면 Comment를 남겨주세요.
- 해당 Comment에 대해서는 자유롭게 답변을 달아 주시면 됩니다.
- 매주 수요일 21시 전에 각자 발표 자료를 PR로 올립니다.
- 매주 수요일 21시에는 한 사람 당 한개씩 아이템 발표를 진행합니다.

### 발표

- 매주 한 사람당 한 개의 아이템을 준비하여 발표를 진행합니다.
- 발표 자료는 당일 02시00분 까지(새벽2시 까지) PR로 올려주세요.
  - 스터디 구성원들의 과도한 야근을 방지하기 위함입니다. ⛑️
- Effective Java에 나오는 예제 코드 외적으로 자신이 생각하는 적절한 예제코드를 작성해주셔야 합니다.
  - Effective Java에 나오는 예제 코드를 발표자료에 포함하셔도 되고, 안해주셔도 됩니다.
  - 그러나 자신만의 예제코드는 꼭 한개씩은 넣어주시길 바라겠습니다.
- 발표자료는 Markdown, PDF,PPT 등 자유롭게 올려주시면 됩니다.
  - but, 최대한 형식에 구애받지 않고, 내용에만 집중하실 수 있는 markdown 을 추천합니다 😃
  - 노션, 타이포라 등등 공유가 간편한 필기App사용도 OK!
- 발표 시간은 10분 내로 준비해주세요. (발표할 때 반드시 해당 아이템의 모든 내용을 담을 필요는 없습니다. )
- 발표는 개인별로 진행합니다.

### Github 저장소

- PR에 대한 머지는 운영진이 할 예정입니다.
- 발표자료의 파일명은 본인의 디렉토리에 알아서 구성하시면 됩니다

```txt
아이템번호_아이템이름_본인이름
```

- PR을 올려주실때는 포크 저장소를 이용해주세요.

### 회고

- 두 팀이 모여 한 공간에서 진행합니다.
- 한명당 2분~3분정도 이야기 해주시면 됩니다.
- 1주일 동안 책을 읽으면서 느낀점, 발표를 보고 느낀점 들을 자유롭게 이야기 해주시면 됩니다.
- 자유롭게 각자 하고 싶은 말을 하면 되니 부담 가지실 필요는 없습니다.

### 보증금 및 벌금
- 다들 좋은사람들이니 일단은 벌금제도는 없어요! : )

```
- 보증금 2만원을 첫 시작 때 운영진에게 입금합니다.
- 발표자료를 기한 내에 PR하지 않은 경우 벌금으로 차감됩니다.
- 벌금은 4000원입니다.
- 마지막 모임에서 남은 금액에 대해 환급을 받습니다..
- 모든 벌금은 마지막 모임 시, 오프라인 모임 시 사용됩니다. (스터디룸 비 및 회식 비)
- 중도 하차하신 분은 보증금을 돌려드리지 않습니다.
  - 한번열면 멈출수 없어! 🐿️
```
- 이런 무시무시한 제도가 운영되지 않도록 제가 더 열심히 노555력 하겠습니다

<br><hr><br>

## Q&A

- 한사람당 하나의 발표는 매주 5개씩 진행하는 아이템 중에 자유롭게 선택하는 걸까요? 그렇다면 중복으로 선택되는 아이템도 생길수 있는 건가요?

  자유롭게 선택은 문제가 될수 있기 때문에, 사다리 타기를 진행할 예정입니다. 그러나 스터디원들끼리 아이템 변경에 대해서는 열어둘 생각입니다.!(예를들면 A와 B가 아이템을 변경해서 준비할 수 있겠죠!? ㅎㅎ)

- 5명이 각 챕터당 1개의 아이템을 지정해서 매주 발표하는 식으로 진행이 되는건가요?

  넵 맞습니다 이번주가 아이템 1 ~ 5이라고 하면 1 ~ 5까지의 지정된 아이템을 하나씩 선택해 매주 발표하는 식입니다.

- 스터디 요일이 토요일인 이유가 있나요?

  평일 공부가 쉽지 않다라는 걸 착안하여, 토요일 오전(10시)으로 일단 가닥을 잡게 되었고 다른 요일보다는 토요일에는 크게 일이 없을거 같은 생각에 잡게 되었습니다.
