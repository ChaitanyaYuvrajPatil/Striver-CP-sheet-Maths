
Problem : Magic Stick (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1257/B

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
       ll x,y;
       cin>>x>>y;

      if(x==1&&y>1) cout<<"NO"<<endl;
      else if(x<=3 && y>3) cout<<"NO"<<endl;
      else cout<<"YES"<<endl;
    }
    return 0;
}
```
