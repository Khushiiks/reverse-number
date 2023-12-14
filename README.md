# reverse-number
//reversing a number using c++
#include <iostream>
using namespace std;
int main()
{
    int n,s=0;
    cin>>n;
    while(n!=0)
    {
        int d=n%10;
        if((s>INT_MAX/10)||(s<INT_MIN/10))
        {
            return 0;
        }
        s=s*10+d;
        n=n/10;
    }
    cout<<s;
}
