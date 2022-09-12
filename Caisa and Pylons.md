
Problem : Caisa and Pylons (Codeforces)

Problem link : https://codeforces.com/problemset/problem/463/B

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   ll t,x,enengy =0 ,prev=0,ans=0;
   cin>>t;

   while(t--)
   {
      cin>>x;
      enengy += prev-x;

      if(enengy<0){
         ans += abs(enengy);
         enengy = 0;
      }
      prev = x;
   }

   cout<<ans<<endl;
   return 0;
}
```
