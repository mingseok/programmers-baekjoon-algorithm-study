Arrays.copyOfRange() 을 이용하여 풀어봤습니다.
```java
import java.util.Arrays;
class Solution {
    public int[] solution(int[] num_list, int n) {
        int[] answer = Arrays.copyOfRange(num_list, n-1, num_list.length);
        return answer;
    }
}
```


for문을 이용하여 풀어봤습니다.
```java
class Solution {
    public int[] solution(int[] num_list, int n) {
        int[] answer = new int[num_list.length-(n-1)];
        int count = 0;
        for(int i=0; i<num_list.length; i++) {
            if(i >= n-1) {
                answer[count] = num_list[i];
                count++;
            }
        }
        return answer;
    }
}
```