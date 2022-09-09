
Problem : Theatre Square (Codeforces)

Problem link : https://codeforces.com/problemset/problem/69/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   ll n,m,a;
   cin>>n>>m>>a;
   ll ans = 0;
   
   ans += (ceil(1.0*n/a)*ceil(1.0*m/a));
   cout<<ans<<endl;
   return 0;
}
```
