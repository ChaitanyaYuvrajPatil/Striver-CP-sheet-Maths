
Problem : Number Circle (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1189/B

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

   vector<ll> vec(n);

   for(int i=0;i<n;i++) cin>>vec[i];
   sort(vec.begin(),vec.end());

   if(vec[n-1] >= vec[n-2]+vec[n-3]) cout<<"NO"<<endl;
   else{
      cout<<"YES"<<endl;
      cout<<vec[n-1]<<" ";
      for(int i=n-3;i>=0;i--) cout<<vec[i]<<" ";
      cout<<vec[n-2]<<endl;
   }
   return 0;
}

```
