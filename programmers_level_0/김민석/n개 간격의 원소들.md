## n개 간격의 원소들

```java
import java.util.List;
import java.util.ArrayList;

class Solution {
    public int[] solution(int[] num_list, int n) {
        List<Integer> arr = new ArrayList<>();
        int count = 1;
        arr.add(num_list[0]);
        
        for(int i = 1; i < num_list.length; i++) {
            if(count == n) {
                arr.add(num_list[i]);
                count = 0;
            }
            count++;
        }
        
        int[] answer = new int[arr.size()];
        for(int i = 0; i < arr.size(); i++) {
            answer[i] = arr.get(i);
        }
        return answer;
    }
}
```