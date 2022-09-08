
Problem :  Digital root (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1107/B

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
       ll k,x;
       cin>>k>>x;

       ll ans = 9*(k-1) + x;
       cout<<ans<<endl;     
    }
    return 0;
}
```
