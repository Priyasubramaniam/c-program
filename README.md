// c-program
// first and last x digits are same
#include<stdio.h>
#include<string.h>
int main()
{
int i,temp,n,len;
char a[1000000];
scanf("%s %d",&a,&n);
len=strlen(a);
temp=len-n;
for(i=0;i<n;i++)
{
if(a[i]!=a[temp+i])
{
printf("No");
return 0;
}
}
printf("Yes");
return 0;
}
