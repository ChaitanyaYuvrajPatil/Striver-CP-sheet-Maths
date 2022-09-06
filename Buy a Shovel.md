
Problem : Buy a Shovel (Codeforces)

Problem link : https://codeforces.com/problemset/problem/732/A


## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
using namespace std;

int main()
{
   
   int k,r;

   cin>>k>>r;

   int m = k;
   for(int i=1;i<=10;i++)
   {
       m = k*i;

       if(m%10 == 0 || m%10 == r)
       {
         cout<<i<<endl;
         return 0;
       }
   }
   return 0;
}
```
