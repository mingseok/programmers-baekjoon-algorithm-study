## A 강조하기

```java
class Solution {
    public String solution(String myString) {
        String answer = "";
        for(Character x : myString.toCharArray()) {
            if(x.equals('a')) {
                answer += Character.toUpperCase(x);
            } else if(x.equals('A')) {
                answer += x;
            } else if(Character.isUpperCase(x)) {
                answer += Character.toLowerCase(x);
            }else {
                answer += x;
            }
        }
        return answer;
    }
}
```