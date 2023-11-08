## 무작위로 K개의 수 뽑기

```java
import java.util.*;

class Solution {
    public int[] solution(int[] arr, int k) {
        List<Integer> list = new ArrayList<>();
        for(int i = 0; i < arr.length; i++) {
            if (list.size() == k) {
                break;
            }

            if (!list.contains(arr[i])) {
                list.add(arr[i]);
            }
        }

        while (list.size() < k) {
            list.add(-1);
        }

        int[] result = new int[k];
        for (int i = 0; i < k; i++) {
            result[i] = list.get(i);
        }

        return result;
    }
}
```