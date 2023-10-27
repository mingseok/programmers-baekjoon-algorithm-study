## 홀수 vs 짝수

```java
class Solution {
    public int solution(int[] num_list) {
        int answer = 0;
        int number = 0;
        for(int i = 0; i < num_list.length; i++) {
            if(!(i % 2 == 0)) {
                answer += num_list[i];
            } else {
                number += num_list[i];
            }
        }
        answer = Math.max(answer, number);
        return answer;
    }
}
```