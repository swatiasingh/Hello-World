# Hello-World

Hello everyone, I have a code to debug and here is it.

#include<stdio.h>
#include<string.h>
int main()
{
	int i,j,k,c,r,p,l;
	char a[201];
	while(1)
	{
		scanf("%d",&c);
		if(c==0)
		break;
		scanf("%s",a);
		p=strlen(a);
		r=p/c;
		char b[r][c];
		l=0;
		for(i=0;i<r;i++)
		{
			if(i%2==0)
			{
			for(j=0;j<c;j++)
			{
				b[i][j]=a[l];
				l++;
			}
			}
			else
			{
			for(k=j-1;k>=0;k--)
			{
				b[i][j]=a[l];
				l++;
			}
			}
		}
		for(i=0;i<c;i++)
		{
			for(j=0;j<r;j++)
			printf("%c",b[j][i]);
		}
	}
	return 0;
}
