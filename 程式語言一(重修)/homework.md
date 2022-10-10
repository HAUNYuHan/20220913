## hw01
```
#include <stdio.h>
#include<stdlib.h>

int main(void){
    printf("%d\n",26);
    printf("%d\n",032);
    printf("%d\n",0x1A);
    
    return 0;
}
```
```
222
336
de

```
## hw02
```
int main(void){
    
    printf("C language\t\t1399.48\n");
    printf("Python language\t\t80.72\n");
    printf("Java Languagr\t\t95.59\n");
    
    
    return 0;
}
```
```
C language              1399.48
Python language         80.72
Java Languagr           95.59
```
## hw03
```
#include <stdio.h>


int main(void){
	char inputA[4];
	float inputB, inputC,inputD;
	
	printf("請鍵入學號:");
	scanf("%s",&inputA);
	
	printf("請鍵入期中考分數:");
	scanf("%f",&inputB);
	
	printf("請鍵入期末考分數:");
	scanf("%f",&inputC);
	
	
	inputD=(inputB+inputC)/2;
	
	printf("\n學號:%s\n",inputA);
	printf("期中分數:%.2f\n",inputB);
	printf("期末分數:%.2f\n",inputC);
	printf("期末考與期中考平均分數:%.2f\n",inputD);
	
	return 0;
} 
```
```
請鍵入學號:e036
請鍵入期中考分數:60
請鍵入期末考分數:100

學號:e036
期中分數:60.00
期末分數:100.00
期末考與期中考平均分數:80.00
```
## hw04
```
#include<stdio.h>
int main()
{
	int x=34,y;
	int result;
	y = 57;
	result = x * (y);
	printf("result = %d  x = %d  y = %d\n", result, x ,y);
    
	y = 6;
	result = x * (y);
	printf("result = %d  x = %d  y = %d\n", result, x, y);
	return 0;
}

```
```
result = 1938  x = 34  y = 57
result = 204  x = 34  y = 6
```
