
Problem : Three Pairwise Maximums (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1385/A

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
        int n;
        vector<int> vec(3);
        cin>>vec[0]>>vec[1]>>vec[2];

        sort(vec.begin(),vec.end());
        
        if(vec[1]!=vec[2]) cout<<"NO"<<endl;
        else{
            cout<<"YES"<<endl;
            cout<<vec[0]<<" "<<vec[0]<<" "<<vec[2]<<endl;
        }
    }
    return 0;
}
```
