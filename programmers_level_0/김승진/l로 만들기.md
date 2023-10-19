```c++
#include <iostream>
#include <string>
#include <vector>

using namespace std;

string solution(string myString){
  string answer = "";
  for (int i = 0; i < myString.size(); i++)
  {
      if (myString[i] < 'l')
      myString[i] = 'l';
  }
  answer = myString;
  cout << answer;
  return answer;
}
```
