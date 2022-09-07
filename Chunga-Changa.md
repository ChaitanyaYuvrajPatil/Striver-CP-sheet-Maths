
Problem :  Chunga-Changa(Codeforces)

Problem link : https://codeforces.com/problemset/problem/1181/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   ll x,y,z,ans = 0,k=0;
   cin>>x>>y>>z;
   ll total = (x+y)/z;
   ll another = x/z + y/z;

   ll a = z- x%z;
   ll b = z -y%z;

   cout<<total<<" ";
   if(total > another)
   {
      cout<<min(a,b)<<endl;
   }
   else{
      cout<<0<<endl;
   }
   return 0;
}
```
