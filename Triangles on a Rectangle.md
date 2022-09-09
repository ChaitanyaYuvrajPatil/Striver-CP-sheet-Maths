
Problem :  Triangles on a Rectangle (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1620/B

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
       ll w,h,n,first,last,p,area =0;
       cin>>w>>h;

       for(int i=0;i<4;i++)
       {
          cin>>n;
          for(int j=0;j<n;j++)
          {
             cin>>p;
             if(j==0) first = p;
             if(j+1 == n) last = p;
          }
          ll base = last - first;

          if(i<2) area = max(area,base*h);
          else area = max(area,base*w);
       }

       cout<<area<<endl;
    }
    return 0;
}
```
