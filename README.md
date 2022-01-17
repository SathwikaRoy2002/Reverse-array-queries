#include <bits/stdc++.h>
#pragma GCC optimize("Ofast")
#pragma GCC optimize("unroll-loops")
#pragma GCC target("avx2")
#pragma GCC optimize("Os")
using namespace std;
#define ll long long
#define ccc ios::sync_with_stdio(0); cin.tie(0); cout.tie(0);
int main(int argc, char const *argv[])
{
    ll n,i,q,a,l,r;
    cin>>n;
    ll arr[n];
    for(i=0;i<n;i++)
    {
        cin>>arr[i];
    }
    cin>>q>>a;
    while(q--)
    {
        cin>>l>>r;
        for(i=0;i<=(r-l)/2;i++)
        swap(arr[l+i],arr[r-i]);
    }
    for(int V:arr)
        cout<<V<<"\n";
    return 0;
}
