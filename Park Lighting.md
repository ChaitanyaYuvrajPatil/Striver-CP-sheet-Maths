
Problem : Park Lighting (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1358/A

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
        int n,m;
        cin>>n>>m;

        long k =n*m;

        if(k%2)
        {
            cout<<(k/2)+1<<endl;
        }
        else{
            cout<<(k/2)<<endl;
        }
    }
    return 0;
}
```
