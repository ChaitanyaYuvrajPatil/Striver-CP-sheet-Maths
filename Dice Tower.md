
Problem :  Dice Tower (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1266/B

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
       ll x;
       cin>>x;
       if(x>14 && x%14>=1 && x%14<=6)
       {
        cout<<"YES"<<endl;
       }
       else{
        cout<<"NO"<<endl;
       }
    }
    return 0;
}
```
