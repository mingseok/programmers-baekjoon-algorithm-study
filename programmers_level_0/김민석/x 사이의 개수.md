## x 사이의 개수

```java
import java.util.List;
import java.util.ArrayList;

class Solution {
    public int[] solution(String myString) {
        List<Integer> arr = new ArrayList<>();
        String[] split = myString.split("x");

        for(int i = 0; i < split.length; i++) {
            arr.add(split[i].length());
        }

        char ch = myString.charAt(myString.length()-1);
        if (ch == 'x') {
            arr.add(0);
        }

        int[] answer = new int[arr.size()];
        for(int i = 0; i < arr.size(); i++) {
            answer[i] = arr.get(i);
        }
        return answer;
    }
}
```