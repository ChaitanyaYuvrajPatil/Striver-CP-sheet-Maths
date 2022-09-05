
Problem :  Balanced Array (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1343/B

Youtube : https://www.youtube.com/watch?v=Ev26R7Cxa3w

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

        if((n/2) % 2)
           cout<<"NO"<<endl;
        else
        {
            cout<<"YES"<<endl;
            ll j = 2;

            for(int i=1;i<=n/2;i++)
            {
                cout<<j<<" ";
                j+=2;
            }

            ll val = j-2;

            j=1;

            for(int i=1;i<n/2;i++)
            {
                cout<<j<<" ";
                j+=2;
            }

            cout<<val+(n/2)-1<<endl;
        }
    }
    return 0;
}
```
