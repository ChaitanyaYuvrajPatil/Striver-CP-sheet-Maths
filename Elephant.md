
Problem : Elephant (Codeforces)

Problem link : https://codeforces.com/problemset/problem/617/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   ll x;
   
   cin>>x;
   ll ans = x/5;
   if(x%5)
   {
      ans++;
      cout<<ans<<endl;
   }
   else{
      cout<<ans<<endl;
   }
   return 0;
}
```
