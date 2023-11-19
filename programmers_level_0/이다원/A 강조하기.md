```Java

class Solution {
    public String solution(String myString) {
        String answer = "";
        for(char x: myString.toCharArray()){
            if(x == 'a' || x == 'A'){
                answer+=Character.toUpperCase(x);
            }else{
                answer+=Character.toLowerCase(x);
            }
        }
        return answer;
    }
}
```
