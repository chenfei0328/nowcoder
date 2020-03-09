C++

```C++
#include <iostream>
using namespace std;

int main() {
    int n;
    cin>>n;
    int count = 0;
    string bad = "347", other = "2569";
    for(int num = 1; num <= n; ++num) {
        string s = to_string(num);
        if(s.find_first_of(bad) == s.npos && s.find_first_of(other) != s.npos) {
            count++;
        }
    }
    cout<<count;
    return 0;
}
```



python3

```python3
def main():
    n = int(input())
    count = 0
    for num in range(1, n + 1):
        s = str(num)
        if ('2' in s or '5' in s or '6' in s or '9' in s) and ('3' not in s and '4' not in s and '7' not in s):
            count += 1
    print(count)

if __name__ == '__main__':
    main()
```

