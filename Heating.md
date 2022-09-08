
Problem :  Heating (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1260/A

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
       ll c,sum;
       cin>>c>>sum;
       ll ans = 0;

       if(c>=sum) cout<<sum<<endl;
       else
       {
          ll x = sum/c;
          ll ext = sum%c;
          if(ext == 0)
          {
            ans += c*(x*x);
          }
          else{
            ans += x*x*(c-ext) + ext*(x+1)*(x+1);
          }

          cout<<ans<<endl;
       }   
    }
    return 0;
}
```
