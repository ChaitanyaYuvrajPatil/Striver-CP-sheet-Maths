
Problem : Yet Another Two Integers Problem (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1409/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
using namespace std;
#define ll long long


int main()
{
    int t;
    cin>>t;

    while(t--)
    {
        ll a,b;

        cin>>a>>b;

        ll dif = abs(b-a);
        int ans = dif/10;

        if(dif%10)
          ans++;

        cout<<ans<<endl;
    }
    return 0;
}
```
