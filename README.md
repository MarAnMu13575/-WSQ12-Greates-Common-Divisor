# -WSQ12-Greates-Common-Divisor
#include iostream>
using namespace std;


int common(int first, int second)
{

	if (first==second)
	{
	
		return first;
	}
	
	else if (first>second)
	{
	
		return common(first-second, second);
	}
	else
	{
	
		return common(first, second-first);
	}
}

int main ()
{
	int x,y;
	
  cout<<"Hello this is the  greatest common divisor from two numbers here we go: "<<endl;
  

  cout<<"Enter the first number, please "<<endl;
  
 
	cin>>x;
  
  
  cout<<"Enter the second number, ¡yeah! "<<endl;

  cin>>y;
  

	cout<<"The greatest common divisor  is "<<common(x,y)<<endl;
	
	return 0;
}
