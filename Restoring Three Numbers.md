
Problem :  Restoring Three Numbers (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1154/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
using namespace std;

int main()
{
   
   vector<int> vec(4);
   cin>>vec[0]>>vec[1]>>vec[2]>>vec[3];
   sort(vec.begin(),vec.end());

   cout<<vec[3]-vec[0]<<" "<<vec[3]-vec[1]<<" "<<vec[3]-vec[2]<<endl;
   return 0;
}
```
