
Problem : Sequence with Digits (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1355/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
using namespace std;
#define ll long long

ll fun(ll a)
{
   ll mx=-1,mn =10;
   while (a>0)
   {
      ll rem = a%10;
      mx = max(mx,rem);
      mn = min(mn,rem);
      a = a/10;
   }
   
   return mx*mn;
}
int main()
{
    ll t;
    cin>>t;

    while(t--)
    {
      ll a,k;
      cin>>a>>k;

      while(--k)
      {
        ll f = a + fun(a);
        if(f==a) break;
        a = f;
      }

      cout<<a<<endl;
    }
    return 0;
}
```
