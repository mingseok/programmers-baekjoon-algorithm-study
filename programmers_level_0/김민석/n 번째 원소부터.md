## n 번째 원소부터


```java
import java.util.Arrays;

class Solution {
    public int[] solution(int[] num_list, int n) {
        int[] answer = new int[num_list.length - n + 1];
        answer = Arrays.copyOfRange(num_list, n - 1, num_list.length);

        return answer;
    }
}
```