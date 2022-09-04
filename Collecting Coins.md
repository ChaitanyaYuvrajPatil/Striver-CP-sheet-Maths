
Problem : Collecting Coins (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1294/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
using namespace std;


int main()
{
    int t;
    cin>>t;

    while(t--)
    {
        vector<int>vec(3);
        int n;

        cin>>vec[0]>>vec[1]>>vec[2]>>n;
        sort(vec.begin(),vec.end());
        
        n = n - (vec[2]-vec[0]);
        n = n - (vec[2]-vec[1]);

        if(n<0 || n%3)
          cout<<"NO"<<endl;
        else
          cout<<"YES"<<endl;
    }
    return 0;
}
```
