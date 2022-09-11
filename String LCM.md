
Problem : String LCM (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1473/B

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
using namespace std;
#define ll long long


int gcd(int a, int b) {
   if (b == 0)
   return a;
   return gcd(b, a % b);
}


int main()
{
    ll t;
    cin>>t;

    while(t--)
    {
      string s1,s2,ans="";
      cin>>s1>>s2;
      ll n = s1.size(),m= s2.size();
      ll lcm = (m*n)/__gcd(n,m);

      string r1="",r2="";
      for(int i=0;i<lcm/n;i++) r1+=s1;
      for(int i=0;i<lcm/m;i++) r2+=s2;

      if(r1==r2) cout<<r1<<endl;
      else cout<<-1<<endl;
    }
    return 0;
}
```
