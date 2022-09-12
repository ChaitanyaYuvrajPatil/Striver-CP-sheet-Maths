
Problem : Road To Zero (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1342/A

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
      ll x,y,a,b;
      cin>>x>>y>>a>>b;

      if(x==0 && y==0) cout<<0<<endl;
      else if (x==0 || y==0) cout<<max(x*a,y*a)<<endl;
      else 
      {
        ll d = 0,temp=0;
         if(x<y)
         {
            d = (y-x);
            temp = d*a + x*b;
         }
         else
         {
            d = (x-y);
            temp = d*a + y*b;
         }
         cout<< min(temp,x*a+y*a)<<endl;
      }
    }
    return 0;
}
```
