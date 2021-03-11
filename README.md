#include<stdio.h>
#include<time.h>
#include<stdlib.h>
void printUnitUpperTriangular(int);
void main()
{
int n;
printf("Enter the size of matrix: ");
scanf("%d",&n);
printUnitUpperTriangular(n);
}
void printUnitUpperTriangular(int Msize){
int i,j;
srand(time(NULL));
for(i=0;i<Msize;i++)
{
	for(j=0;j<Msize;j++)
	{
		if(i==j)
		{
			printf("1 ");
		}
		else if (i>j)
		{
			printf("0 ");
		}
		else 
		{
			printf("%d ", rand()%(Msize + 1));
		}
	}
	 printf("\n");
}
}
