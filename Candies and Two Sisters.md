
Problem : Candies and Two Sisters (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1335/A

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
        ll n;

        cin>>n;

        ll ans = n/2;
        if(n<=2) cout<<0<<endl;
        else if(n%2)
        {
            cout<<ans<<endl;
        }
        else{
            ans--;
            cout<<ans<<endl;
        }

    }
    return 0;
}
```
