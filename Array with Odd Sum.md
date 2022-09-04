
Problem : Array with Odd Sum (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1296/A

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
        int n,sum=0,od=0,ev=0;
        cin>>n;

        for(int i=0;i<n;i++)
        {
            int k;
            cin>>k;
            sum+=k;

            if(k%2 == 0) ev++;
            else od++;
        }

        if(sum%2) cout<<"YES"<<endl;
        else{
            if(od>=1 && ev>=1)
               cout<<"YES"<<endl;
            else
               cout<<"NO"<<endl;
        }
    }
    return 0;
}
```
