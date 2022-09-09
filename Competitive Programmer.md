
Problem :  Competitive Programmer (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1266/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
using namespace std;
#define ll long long


int main()
{
    ll t;
    cin>>t;

    while(t--)
    {
       ll even = 0,sum=0,zero = 0;
       string s;
       cin>>s;

       for(int i=0;i<s.size();i++)
       {
          int k = s[i] - '0';

          if(k == 0) zero = 1;
          if(k%2 == 0) even++;
          sum+=k;
       }

       if(zero && even>1 && sum%3==0) cout<<"red"<<endl;
       else cout<<"cyan"<<endl;
    }
    return 0;
}
```
