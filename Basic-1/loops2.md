## 1.Given an input, print digits of number from right(LSD) to left(MSD) as space separated.
### inp: 6749 out: 9 4 7 6
```c
#include <stdio.h>
#include <string.h>

int main() {
    char str[] = "6749";

    int len = strlen(str);

for(int i=len;i>=0;i--){
    printf("%c ",str[i]);
}
    return 0;
}
```
## 2.Given an input, print digits of number from left(MSD) to right(LSD)   as space separated.
### inp: 6749 out: 6 7 4 9
```c
#include <stdio.h>
#include <string.h>

int main() {
    char str[] = "6749";

    int len = strlen(str);

for(int i=0;i<len;i++){
    printf("%c ",str[i]);
}
    return 0;
}
```
## 3.Given an input, count number of digits.
### inp:6749 out:4
```c
#include <stdio.h>
#include <string.h>

int main() {
    char str[] = "6749";

    int len = strlen(str);

printf("%d",len);
    return 0;
}
```
## 4.Given an input, find sum  of digits.
### inp:6749 out:26
```c
#include <stdio.h>
#include <string.h>

int main() {
    char str[] = "6749";
int sum=0;
    int len = strlen(str);
for(int i=0;i<len;i++){
    sum+=str[i]-'0';
}
printf("%d",sum);
    return 0;
}
```
## 5.Given an input, print even digits followed by odd digits.
### inp:12345678 out:13572468
```c
#include <stdio.h>
#include <string.h>

int main() {
   char str[]="12345678";
   
    int out;
    int out1;
    int len = strlen(str);
for(int i=0;i<len;i++){
    int d=str[i]-'0';
    if(d%2!=0)
    printf("%d",d);
   
}
for(int i=0;i<len;i++){
    int d=str[i]-'0';
    if(d%2==0)
    printf("%d",d);  
}
}
```
## 6.Armstrong number
Given an input, find number of digits of the given input, and raise the power of each digit to number of digit times and sum those values, if the sum is equal to the input, its Armstrong number
### inp: 153 out:yes exp:1^3+5^3+3^3=153
```c
#include <stdio.h>
#include <math.h>

int main()
{
    int n = 153;
    int original = n;
    int c = 0, sum = 0;

    // Count digits
    while (n > 0) {
        c++;
        n = n / 10;
    }

    n = original;  // restore original value

    // Calculate Armstrong sum
    while (n > 0) {
        int digit = n % 10;
        sum += pow(digit, c);
        n = n / 10;
    }

    printf("%d", sum);
}
```
## 8.Given an input, segregate even digits to the left followed by odd digits, store the result in one variable and print it. dont use arrays/strings.
### inp:7632541	out:6247351
```c
#include <stdio.h>
int main()
{
    int n=2345678;
    for(int i=1;i<=n%10;i++){
        if(i%2==0){
            printf("%d",i);
        }
    }
     for(int i=1;i<=n%10;i++){
        if(i%2!=0){
            printf("%d",i);
        }  
    }
    
    return 0;
}
```
## 9.Given an input, do swap digits as pairs.
### inp:723641589 out: 732465198

```c
#include <stdio.h>
int main()
{
    int n=12345678;
    int res=0; 
    int place=1;
    while(n>=10){
        int dig1=n%10;
        n=n/10;
        int dig2=n%10;
        n=n/10;
        int swap=dig1*10+dig2;
        res=res+swap*place;
        place*=100;
        
    }
   
    printf("%d",res);
    
    return 0;
}
```

## 10.Given two inputs, check first input is rotated version of the second or not.
### inp: 12345 34512 out:yes 
inp: 12345 45312 out:no

```c
#include <stdio.h>
int main()
{
    int n=12345;
    int k=34521;
    int c=0;
    int o=n;
    while(n>0){
        c++;
        n/=10;
    }
     n=o;
    int m=(c+1)/2;
   
    int p=(n/100)/10;
    
  int result = 0;

result = result * 10 + m;
result = result * 10 + (m + 1);
result = result * 10 + (m + 2);
result = result * 100 + p;

if(result==k){
    printf("yes");
}
else printf("no");
    
    return 0;
}
```
