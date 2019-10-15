#include<iostream>
#include<math.h>
using namespace std;
int main()
{
int n,p,rem, res=0,i=0;
cout <<"enter a number"<<"\n";
cin>>n;
p=n;
while(p!=0)
{
p/=10;
++i;
}
p=n;
while(p!=0)
{
rem=p%10;
res+=pow(rem,i);
p/=10;
}
if(res==n)
cout<<"IT is an Armstrong number";
else
cout <<"IT is not an Armstrong number";
}
