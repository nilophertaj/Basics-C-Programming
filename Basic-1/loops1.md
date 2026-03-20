## 1. Given a start and end of a range, print the numbers that 	are 7's 	multiple in that range. 
### inp :10 30 out:14 
```c
#include <stdio.h>

int main()
{
   int n,m;
   printf("enter the two nos: ");
   scanf("%d %d",&n,&m);
   for(int i=n;i<m;i++){
       if(i%7==0)
       printf("%d ",i);
   }
   
    return 0;
}
```
## 2. Given a range, print even numbers in the range.
### inp: 10 out: 2 4 6 8 10
```c
#include <stdio.h>

int main()
{
   int m;
   printf("enter the no: ");
   scanf("%d",&m);
   for(int i=2;i<=m;i++){
       if(i%2==0)
       printf("%d ",i);
   }
   
    return 0;
}
```

## 3. Given an N, print first N odd numbers. 
### inp:3 out: 1 3 5
```c
#include <stdio.h>

int main()
{
   int n;
   printf("enter the no: ");
   scanf("%d",&n);
   for(int i=1;i<=n;i++){
          printf("%d ",2*i-1);    
   }
   
    return 0;
}
```
## 4. Given an input, find sum of numbers in that range.
### inp: 4 out: 1 3 6 10 exp: 1+2+3+4
```c
#include <stdio.h>

int main()
{
   int n;
   printf("enter the no: ");
   scanf("%d",&n);
   int sum=0;
   for(int i=1;i<=n;i++){
      
        sum+=i;
        printf("%d ",sum); 
   }
   
    return 0;
}
```
### Another method ( Print only the final output)
### inp: 4 out: 10 exp: 1+2+3+4
```c
#include <stdio.h>

int main()
{
   int n;
   printf("enter the no: ");
   scanf("%d",&n);
   int sum=0;
   for(int i=1;i<=n;i++){
        sum+=i;    
   }
   printf("%d ",sum);
   
    return 0;
}
```
### Note : if printf statement present inside the loop then it prints for every iteration. To get one single output then put printf statement outside the loop.

## 5. Given two number multiply two numbers without using '*' operator.
### inp: 3 7 out: 21
```c
#include <stdio.h>

int main()
{
   int n,m;
   printf("enter the 2 nos: ");
   scanf("%d %d",&n,&m);
int sum=0;
   for(int i=1;i<=n;i++){
      sum+=m;   
   }
   printf("%d",sum);
   
    return 0;
}
```
## 6.Given an input, find factorial of it.  
### inp: 5 out:120 exp:5*4*3*2*1
```c
#include <stdio.h>

int main()
{
   int n;
   printf("enter the no: ");
   scanf("%d",&n);
int mul=1;
   for(int i=n;i>=1;i--){
      mul=mul*i;     
   }
   printf("%d",mul);
   
    return 0;
}
```

## 7.Given two number, raise the power of first number to other, without using inbuilt power function.
### inp: 5 3 out:125 exp:5^3=>125
```c
#include <stdio.h>

int main()
{
   int n,m;
   printf("enter the 2 nos: ");
   scanf("%d %d",&n,&m);
int mul=1;
   for(int i=1;i<=n;i++){
      mul=mul*m;   
   }
   printf("%d",mul);
   
    return 0;
}
```
## 8.Given table_num and no_times print the multiplication table for the given 	no_times.  
### inp:3 5  out:
	1 X 3 = 3
	2 X 3 = 6
	3 X 3 = 9
	4 X 3 = 12
	5 X 3 = 15
```c
#include <stdio.h>

int main()
{
   int n,m;
   printf("enter the 2 nos: ");
   scanf("%d %d",&n,&m);
int mul;
   for(int i=1;i<=n;i++){
      mul=i*m;
       printf("%d x %d = %d\n",i,m,mul);
   }
  
    return 0;
}
```
## 9.Given times, print a-z for given number of times.
### inp:2 output:
```c
abcdefghijklmnopqrtsuvwxyz
abcdefghijklmnopqrtsuvwxyz
```
```c
#include <stdio.h>

int main()
{
   int n;
   printf("enter the no: ");
   scanf("%d",&n);
char a=97,z=122;
   for(int i=1;i<=n;i++){
      for (int j=a;j<=z;j++){
          printf("%c",j);
      }
printf("\n");
   }
  
    return 0;
}
```
## 10.Given a range, find sum of numbers divisible by 3 or 5 in that 
range. 
### inp: 30  out: 225 exp:3+5+6+9+10+12+15+18+20+21+24+25+27+30
```c
#include <stdio.h>

int main()
{
   int n;
   printf("enter the no: ");
   scanf("%d",&n);
int sum=0;
   for(int i=1;i<=n;i++){
     if((i%3 && i%5)==0){
         sum=sum+i;
     }
      
   }
  printf("%d",sum);   
    return 0;
}
```
