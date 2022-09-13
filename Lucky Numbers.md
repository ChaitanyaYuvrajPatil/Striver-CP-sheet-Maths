
Problem : Lucky Numbers (Codeforces)

Problem link : https://codeforces.com/problemset/problem/630/C

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

   ll sum=0,k=2;

   for(int i=0;i<n;i++)
   {
      sum+=k;
      k=k*2;
   }
   cout<<sum<<endl;
   return 0;
}
```
