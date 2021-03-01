# 2021
## 她媽我本帳被盜了
## 回家作業 實習課的 8 題

## 第一題 找零錢
```C
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	printf("%d=50*%d+5*%d+1*%d\n",n,n/50,n%50/5,n%50%5/1);
}
```
## 第二題 因數個數
```C
#include <stdio.h>
int main()
{
	int n,a=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i++)
	{
		if(n%i==0)
		a++;
	}
	printf("%d\n",a);
}
```
## 第三題 找倍數
```C
#include <stdio.h>
int main()
{
	int a[10],ans=0;
	for (int i=0;i<10;i++)
	{
		scanf("%d",&a[i]);

	}
	for(int i=0;i<10;i++)
	{
		if(a[i]%3==0)
		ans++;
	}

	printf("%d\n",ans);
}
```

## 第四題 整數轉換為等級
```C
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	if(n>=90)printf("A\n");
	else if(n<90 && n>=80)printf("B\n");
	else if(n<80 && n>=60)printf("C\n");
	else printf("F\n");
}
```
!(https://i1.kknews.cc/SIG=2ru26a9/ctp-vzntr/15301131549198023s8q5n0.jpg)
