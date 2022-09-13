
Problem : GCD Length (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1511/B

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
      ll a,b,c,x,y,z;
      cin>>a>>b>>c;

      z = pow(10,c-1);
      x = z,y=z;
      while(to_string(x).size()<a) x = x*2;
      while(to_string(y).size()<b) y = y*3;

      cout<<x<<" "<<y<<endl;
    }
    return 0;
}

```
