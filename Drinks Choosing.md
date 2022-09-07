
Problem : A. Drinks Choosing (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1195/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   ll n,k,x;
   cin>>n>>k;
   vector<int>dp(k+1,0);

   int cap = ceil(1.0*n/2);
   for(int i=0;i<n;i++)
   {
      cin>>x;
      dp[x]++;
   }

   int od=0,ev=0;
   for(int i=0;i<=k;i++)
   {
      if(dp[i]%2) ev+=dp[i]-1, od++;
      else ev += dp[i];
   }

   int res=0;
   res+=2*min(ev/2,cap);
   cap-=min(ev/2,cap);
   res+=cap;
   cout<<res;

   return 0;
}
```
