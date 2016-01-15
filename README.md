# count-7
#include<stdio.h>
int c7(n)
{
if(n==0)
return 0;
if(n%10==7)
return 1+c7(n/10);
return c7(n/10);
}
void main()
{
int in,count=0;
scanf("%d",&in);
count=c7(in);
printf("%d",count);
}
