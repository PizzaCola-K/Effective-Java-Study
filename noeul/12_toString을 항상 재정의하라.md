

# toString을 항상 재정의하라



### `toString`은 해당 객체에 관한 명확하고 유용한 정보를 읽기 좋은 형태로 반환해야 한다.



```java
...
    
System.out.println(codeSqaud.toString());


-------------------------------------------------
com.example.Solution$CodeSqaud@2f0e140b
-------------------------------------------------
CodeSqaud{members=[노을, 동, 연, 파이로, K, 어거스트]}
```



## toStirng을 구현할 때면 반환값의 포맷을 문서화할지 정해야 한다. 

### -  🤔 단, 포맷을 명시하든 아니든 의도는 명확히 밝혀야 한다.



### 포맷을 명시하지 않고 작성한 경우

- IDE의 자동완성 기능으로 생성된 toString

```java
public class Solution {

    private static class PhoneNumber {
        final int areaCode;
        final int prefix;
        final int lineNumber;

        public PhoneNumber(int areaCode, int prefix, int lineNumber) {
            this.areaCode = areaCode;
            this.prefix = prefix;
            this.lineNumber = lineNumber;
        }
        
       @Override
        public String toString() {
            return "PhoneNumber{" +
                    "areaCode=" + areaCode +
                    ", prefix=" + prefix +
                    ", lineNumber=" + lineNumber +
                    '}';
        }
    }

    public static void main(String[] args) {
        Map<PhoneNumber, String> map = new HashMap<>();
        map.put(new PhoneNumber(010, 2546, 6893), "박산희");

        System.out.println(map);
    }
}
```



- 포맷에 맞춰 코딩하거나 특정 값을 빼내어 영구 저장한 프로그래머는 나중에 포맷이 바뀌어 피해를 입을 수 있음.

```
{PhoneNumber{areaCode=707, prefix=867, lineNumber=5309}=제니}
```



#### 장점

> 향후 릴리스에서 정보를 더 넣거나 포맷을 개선할 수 있는 유연성을 얻게 된다.????
>
> (🛑 약간, 이해 못한 부분)



#### 단점

> 클래스의 `의미`까지 파악하지 못한다. ?



### 포맷을 명시한 경우

```java
/*
	전화번호의 문자열 표현을 반환
	문자열은 XXX-YYY-ZZZZ 형태의 12글자로 구성
	XXX: 지역코드, YYY: 프리픽스, ZZZZ: 가입자 번호 
	...
*/

@Override
public String toString() {
    return String.format("%03d-%04d-%04d", areaCode, prefix, lineNumber);
}
```

```
{707-0867-5309=제니}
```



#### 장점

>  포맷을 명시하면 그 객체는 표준적이고, 명확하고, 사람이 읽을 수 있게 된다.
>  따라서 그 값 그대로 입출력에 사용하거나 CSV 파일처럼 사람이 읽을 수 있는 객체로 저장할 수도 있다.
>
> 포맷을 명시하기로 했다면, 명시한 포맷에 맞는 문자열과 객체를 상호 전환할 수 있는 `정적 팩토리`나 `생성자`를 함께 제공해주면 좋다.



#### 단점

> 향후 릴리스에서 포맷을 바꾼다면 이를 사용하던 코드들과 데이터들은 엉망이 될 것이다.