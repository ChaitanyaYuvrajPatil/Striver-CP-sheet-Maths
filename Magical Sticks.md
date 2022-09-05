
Problem : Magical Sticks (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1371/A

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
        ll k;
        cin>>k;
        if(k<=2) cout<<1<<endl;
        else
        {
            cout<<1+(k-1)/2<<endl;
        }
    }
    return 0;
}

```
