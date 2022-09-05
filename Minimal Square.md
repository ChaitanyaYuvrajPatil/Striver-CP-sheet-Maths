
Problem : Minimal Square (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1360/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
using namespace std;
#define ll long long


int main()
{
    int t;
    cin>>t;

    while(t--)
    {
        ll a,b;
        cin>>a>>b;

        if(a<b) a = a*2;
        else b = b*2;
        cout<<max(a,b)*max(a,b)<<endl;
    }
    return 0;
}

```
