
Problem : A. LCM Problem (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1389/A

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
        int l,r;
        cin>>l>>r;

        int a = l,b=2*l;
        if(b<=r)
           cout<<a<<" "<<b<<endl;
        else
           cout<<-1<<" "<<-1<<endl;
    }
    return 0;
}

```
