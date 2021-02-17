#include<iostream>
#include<vector>
#include<bits/stdc++.h>
using namespace std;

int main()
{
	int p,d,m,bud;
	cin>>p>>d>>m>>bud;
	int sum=0,count=0;
	
	while(sum<=bud)
	{
		if(p<m)
		{
			sum=sum+m;
			count++;
		}
		else
		{
			sum=sum+p;
			p=p-d;
			count++;
		}
	}
	cout<<count-1<<endl;
	return 0;
}
