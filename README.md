# addition-of-two-complex-number-taking-input-from-user



#include<iostream>
using namespace std;
class complex
{ private:
	int a;
	int b;
	public:
	void getdata(int x,int y)
	{	a=x;
		b=y;
	}
	void showdata(void) 
	{cout<<"a="<<a<<" "<<"b="<<b<<"\n";
		}
   complex add (complex c)
{
	complex temp;
	temp.a=a+c.a;
	temp.b=b+c.b;
	return (temp);
}};
int main()
{ int n,m,p,q;
	complex c1,c2,c3;
	cout<<"enter 1st complex number";
	cin>>n>>m;
	c1.getdata(n,m);
	c1.showdata() ;
		cout<<"enter 2nd complex number";
	cin>>p>>q;
	c2.getdata(p,q);
	c2.showdata() ;
	c3=c1.add(c2);
	c3.showdata() ;
	return 0;
}
