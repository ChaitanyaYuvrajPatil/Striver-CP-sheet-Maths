
Problem :  Even Array (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1367/B

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
        int n,m1=0,m2=0;
        cin>>n;

        for(int i=0;i<n;i++)
        {
            int k;
            cin>>k;

            if(i%2 == 0 && k%2 != 0) m1++;
            else if(i%2 != 0 && k%2 == 0) m2++;
        }

        if(m1 != m2) 
           cout<<-1<<endl;
        else 
           cout<<m1<<endl;
    }
    return 0;
}

```
