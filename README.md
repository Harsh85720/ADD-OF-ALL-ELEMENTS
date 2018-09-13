# ADD-OF-ALL-ELEMENTS
#include<stdio.h>
#include<conio.h>
#include<stdlib.h>
void main()
{clrscr();
int i,j,k,M1[5][5],n,Sum[5],sum=0;
printf("Enter the order of matric:");
scanf("%d",&n);
for(i=0;i<n;i++)
{
      for(j=0;j<n;j++)
      {printf("M1[%d][%d]=",i,j);
      scanf("%d",&M1[i][j]);
      if(M1[i][j]==123)
      {exit(0);}
      }
}
for(i=0;i<n;i++)
{
	Sum[i]=0;
	for(j=0;j<n;j++)
	{
	Sum[i]=Sum[i]+M1[i][j];
	}
	printf("Sum[%d]=%d ",i,Sum[i]);
}
for(i=0;i<n;i++)
{sum=sum+Sum[i];}
printf("\nSum of whole matrix: %d",sum);
getch();
}
