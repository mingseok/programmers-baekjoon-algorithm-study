## StringTokenizer 예시

StringTokenizer의 디폴트는 문자열을 띄어쓰기 기준으로 분리한다.

- nextToken() 메서드로 각각 확인 가능하다.




```java
import java.util.StringTokenizer;
 
public class Main {
    public static void main(String[] args)  {
 
        String str = "안녕하세요 개발자 김민석 입니다.";
        StringTokenizer st = new StringTokenizer(str);
        
        while (st.hasMoreTokens()) {
            System.out.println(st.nextToken());
        }
    }
}


-- 출력값 --
안녕하세요
개발자
김민석
입니다.
```

<br/><br/>


## 띄어쓰기가 아닌 다른 기준으로 잡고 싶을 경우. -> `!`

```java
import java.util.StringTokenizer;
 
public class Main {
    public static void main(String[] args)  {
 
        String str = "오늘!하루도!파이팅";
        StringTokenizer st = new StringTokenizer(str, "!" );
 
        while (st.hasMoreTokens()) {
            System.out.println(st.nextToken());
        }
 
    }
}


-- 출력값 --
오늘
하루도
파이팅
```

<br/><br/>


## 구분자도 같이 출력 시키고 싶은 경우는?


```java
import java.util.StringTokenizer;
 
public class Main {
    public static void main(String[] args)  {
 
        String str = "오늘!하루도!파이팅";
        StringTokenizer st = new StringTokenizer(str, "!", true);
        
        while (st.hasMoreTokens()) {
            System.out.println(st.nextToken());
        }
 
    }
}


-- 출력값 --
오늘
!
하루도
!
파이팅
```
