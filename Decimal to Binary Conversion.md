#include<iostream>
using namespace std;

void bit(int n)
{
    int r,a[10000],i=0;
    while(n!=0)
    {
        r=n%2;
        a[i]=r;
        n=n/2;
        i++;
    }
    for(int j=i;j>=0;j--)
    {
        cout<<a[j];
    }
    cout<<" "<<i-1;
}

int main()
{
    int n;
    cin>>n;
    bit(n);
    return 0;
}
