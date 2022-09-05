
Problem :  Required Remainder (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1374/A

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
        int x,y,n;
        cin>>x>>y>>n;

        int k = n%x;
        if(k-y >= 0)
           n = n-(k-y);
        else
           n = n-k-x+y;
        
        cout<<n<<endl;
    }
    return 0;
}

```
