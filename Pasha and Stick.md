
Problem :  Pasha and Stick (Codeforces)

Problem link : https://codeforces.com/problemset/problem/610/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   ll n,cnt=0;
   cin>>n;
   if(n%2)
   {
      cout<<0<<endl;
      return 0;
   }
   ll k = n/2;

   for(int i=1;i<k;i++)
   {
      if(k-i > i) cnt++;
   }

   cout<<cnt<<endl;
   return 0;
}
```
