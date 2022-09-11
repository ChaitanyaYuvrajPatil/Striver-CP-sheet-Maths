
Problem : Boboniu Likes to Color Balls (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1395/A

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
       ll r,g,b,w,od =0;
       cin>>r>>g>>b>>w;

       if(r%2) od++;
       if(g%2) od++;
       if(b%2) od++;
       if(w%2) od++;

       if(od == 2 || od>=3&&(r==0||g==0||b==0))
       {
        cout<<"NO"<<endl;
       }
       else 
         cout<<"YES"<<endl;
    }
    return 0;
}
```
