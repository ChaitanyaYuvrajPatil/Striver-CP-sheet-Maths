
Problem : Berland Poker (Codeforces)

Problem link : https://codeforces.com/problemset/problem/1359/A

## Solution

```C++
#include<iostream>
#include<bits/stdc++.h>
using namespace std;
#define ll long long

int main()
{
    ll t;
    cin>>t;

    while(t--)
    {
      ll n,m,k;
      cin>>n>>m>>k;

      ll card = n/k;

      if(card>=m) cout<<m<<endl;
      else
      {
         ll rem= m-card;
         ll other = ceil(1.0*rem/(k-1));
         cout<<card-other<<endl;
      }
    }
    return 0;
}

```
