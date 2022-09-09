
Problem : Water Lily (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1199/B

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   double h,l;
   cin>>h>>l;
   cout<<fixed<<setprecision(13)<<(l*l-h*h)/(2*h)<<endl;
   return 0;
}
```
