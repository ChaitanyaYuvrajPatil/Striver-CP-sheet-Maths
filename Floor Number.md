
Problem : A. Floor Number (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1426/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
using namespace std;


int main()
{
    int t;
    cin>>t;

    while(t--)
    {
        int n,x;
        cin>>n>>x;

        if(n<=2)
        {
            cout<<1<<endl;
        }
        else{
            n = n-2;

            int ans = ceil((1.0*n)/x) ;
            cout<<ans+1<<endl;
        }
    }
    return 0;
}

```
