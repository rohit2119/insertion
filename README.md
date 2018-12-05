#include<stdio.h>
int main()
{
int a[100],i,j,n,temp;
printf("enter size");
scanf("%d",&n);
printf("enter elements");
for(i=0;i<n;i++)
{
scanf("%d",&a[i]);
}
for(i=1;i<n;i++)
{
temp=a[i];
j=i-1;
while((j>=0)&&(a[i]>temp))
{
a[j+1]=a[j];
j=i-1;
}
a[j+1]=temp;
}
printf("resultant insertion sort");
for(i=0;i<n;i++)
{
printf("%d \n ",a[i]);
}
}
# insertion
