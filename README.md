# challenge-7
查询座位号

#include <iostream>
using namespace std;
struct students
{
	char num[17];
	int js;
	int ks;
}ren[1000];
int main()
{
	
	int n;
	cin>>n;
	int i;
	for(i=0;i<n;i++) 
		cin>>ren[i].num>>ren[i].js >>ren[i].ks ;
	int m;
	cin>>m;
	int a[1000];
	for(i=0;i<m;i++)
		cin>>a[i];
	
	for(i=0;i<m;i++)
	{
		for(int j=0;j<n;j++)
		{
			if(a[i]==ren[j].js )
			{
				cout<<ren[j].num<<" "<<ren[j].ks <<endl;
				break;
			}
		}
		
	} 
	return 0;
}









