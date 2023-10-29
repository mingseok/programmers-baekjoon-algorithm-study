```c++
#include <string>
#include <vector>

using namespace std;

vector<int> solution(vector<int> num_list, int n) {
    vector<int> answer;
    int prev = 0;
    answer.push_back(num_list[0]);
    for(int i = 1; i < num_list.size();i++){
        if((i - prev) == n){
            answer.push_back(num_list[i]);
            prev = i;
        }
    }
    return answer;
}
```
