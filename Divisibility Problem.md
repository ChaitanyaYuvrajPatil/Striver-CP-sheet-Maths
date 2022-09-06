
Problem : Divisibility Problem (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1328/A

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
        ll a,b,k,i=1;
        cin>>a>>b;

        if(a%b==0)
        {
            cout<<0<<endl;
        }
        else 
        {
            cout<<b-(a%b)<<endl;
        }
    }
    return 0;
}
```
