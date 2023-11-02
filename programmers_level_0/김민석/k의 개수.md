## k의 개수

```java
class Solution {
    public int solution(int i, int j, int k) {
        StringBuilder sb = new StringBuilder();

        for(int z = i; z <= j; z++) {
           sb.append(z);
        }
        String str = sb.toString();
        String[] split = str.split("");
        
        int answer = 0;
        String sss = String.valueOf(k);
        
        for(String x : split) {
            if(x.equals(sss)) {
                answer++;
            }
        }
        return answer;
    }
}
```