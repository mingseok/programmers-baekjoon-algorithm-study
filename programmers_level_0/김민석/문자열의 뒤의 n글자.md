## 문자열의 뒤의 n글자

```java
class Solution {
    public String solution(String my_string, int n) {
        String answer = "";
        int cnt = my_string.length() - n;
        answer = my_string.substring(cnt, my_string.length());
        
        return answer;
    }
}

```