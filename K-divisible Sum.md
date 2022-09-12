
Problem : K-divisible Sum (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1476/A

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
      double n,k;
      cin>>n>>k;
      ll fact = ceil(n/k);
      k = k*fact;
      int ans = ceil(k/n);
      cout<<ans<<endl;
    }
    return 0;
}

```
