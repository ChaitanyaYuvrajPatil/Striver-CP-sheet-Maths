
Problem : Dungeon (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1463/A

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
      ll a,b,c;
      cin>>a>>b>>c;
      ll sum = a+b+c;
      ll k = sum/9;

      if(sum%9 == 0 && a>=k && b>=k && c>=k)
        cout<<"YES"<<endl;
      else 
         cout<<"NO"<<endl;
    }
    return 0;
}
```
