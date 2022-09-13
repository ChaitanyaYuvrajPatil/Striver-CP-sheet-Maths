
Problem : Non-Coprime Partition (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1038/B

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

   if(n<=2) cout<<"No"<<endl;
   else{
      cout<<"Yes"<<endl;
      cout<<2<<" "<<1<<" "<<n<<endl;
      cout<<n-2<<" ";

      for(int i=2;i<n;i++) cout<<i<<" ";
   }
   return 0;
}

```
