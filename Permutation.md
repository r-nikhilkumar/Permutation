#include<iostream>
using namespace std;

int fact(int a)
{
	static int n;
	if (a<=1)
	return 1;
	
	else{
		n= a*fact(a-1);
		return n;
	}
}

int main()
{
	int n,r, p;
	cout<<"Enter the value of n and r respectively :- "<<endl;
	cin>>n>>r;
	p=fact(n)/(fact(r)*fact(n-r));
	cout<<"Your permutation value is :- "<<p;
	
}
