
Problem : Young Physicist (Codeforces)

Problem link : https://codeforces.com/problemset/problem/69/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   ll n,a,b,c;
   cin>>n;

   ll x=0,y=0,z=0;
   for(int i=0;i<n;i++)
   {
      cin>>a>>b>>c;
      x+=a,y+=b,z+=c;
   }

   if(x==0 && y==0 && z==0)
       cout<<"YES"<<endl;
   else
       cout<<"NO"<<endl;
   
   return 0;
}
```
