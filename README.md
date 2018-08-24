#include<stdio.h>

int main(int argc,char *argv[])
{
    int b,n,sum=0,i,rem;
    b=atoi(argv[1]);
    n=b;
    while(b!=0)
    {
        rem=b%10;
        i=fact(rem);
        sum=sum+i;
        b=b/10;
    }
    if(sum==n)
    printf("strong number");
    else
    printf("not strong number");
    return 0;
}
   int fact(int a)
   {
       int fac=1,i;
       if(a==0)
       {
           return fac;
       }
       else
       {
      for(i=a;i>=1;i--)
       fac=fac*i;
       }
       return fac;
   }
    
