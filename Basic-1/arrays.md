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
