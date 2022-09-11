
Problem : Drazil and Date (Codeforces)

Problem link : https://codeforces.com/problemset/problem/515/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   ll a,b,d;
   cin>>a>>b>>d;

   ll ex = d - abs(a)-abs(b);

   if(ex < 0 or ex%2) cout<<"NO"<<endl;
   else cout<<"YES"<<endl;

   return 0;
}

```
