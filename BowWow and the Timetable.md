
Problem : BowWow and the Timetable (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1204/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   string s;
   cin>>s;
   ll n = s.size(),cnt=0;
   ll ans = n/2;

   if(n%2==0)
   {
      cout<<ans<<endl;
      return 0;
   }
   else{
      for(auto it : s)
      {
         if(it == '1') cnt++;
      }
      if(cnt>1) ans++;
      cout<<ans<<endl;
   }

   return 0;
}
```
