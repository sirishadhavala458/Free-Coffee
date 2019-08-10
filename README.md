# Free-Coffee
The coffee shop that you use often has a service that is limited today.  - When purchasing coffee, the price for the next purchase will be P% off. - Truncation after decimal point in each price reduction  You have noticed that the price cuts are cumulative. If you drink coffee many times, you will be able to drink coffee for free.  You want to drink coffee for free, so you will calculate how many INR you can pay for later.


#include<stdio.h>
#include<stdlib.h>
int main()
{
   int x,p,sum=0,count=0;
   printf("Enter the coffee price and value of p\n");
   scanf("%d%d",&x,&p);
   p=100-p;
   while(x!=0)
   {
       sum=sum+x;
       x=(p*x)/100;
       count++;
   }
   printf("%d\n",sum);
   printf("Number of coffee:%d",count);
   return 0;
}
