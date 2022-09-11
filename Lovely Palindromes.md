
Problem : Lovely Palindromes (Codeforces)

Problem link : https://codeforces.com/problemset/problem/688/B

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
#define ll long long
using namespace std;

int main()
{
   string s;
   cin>>s;

   string rev = s;
   reverse(rev.begin(),rev.end());

   cout<<s+rev<<endl;
   return 0;
}
```
