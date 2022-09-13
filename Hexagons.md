
Problem : Hexagons! (Codeforces)

Problem link : https://codeforces.com/problemset/problem/630/D

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   ll n;
   cin>>n;
   ll ans = (3*n*(n+1)) +1;

   cout<<ans<<endl;
   return 0;
}
```
