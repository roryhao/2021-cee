## 第一題 奇數反流 
```c
#include <stdio.h>
int main()
{
	int n;
	int a[100];
	scanf("%d",&n);
	for(int i=1;i<=n;i++)
	{
		scanf("%d",&a[i]);
	}
	for(int i=n;i>=1;i--)
	{
		if(a[i]%2!=0)
		printf("%d ",a[i]);
	}
}
```

## 第二題 大位王 
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	if(n<0)n=-n;
	while(n/10>0)
	{
		n/=10;
	}
	printf("%d\n",n);
}
```

## 第三題 輸入西元y年，判斷該y年是否為閏年
```c
#include <stdio.h>
int main()
{
	int y;
	scanf("%d",&y);
	if(y%4==0 && y%100!=0)printf("%d is a leap year.\n",y);
	else printf("%d is not a leap year.\n",y);
}
```

## 第四題 把數字倒著印出來
```c
#include <stdio.h>
int main()
{
	int a[10];
	for(int i=0;i<10;i++)
	{
		scanf("%d",&a[i]);
	}
	for(int i=9;i>=0;i--)
	{
		printf("%d ",a[i]);
	}
}
```

## 第五題 區間測速 
```c
#include <stdio.h>
int main()
{
	int s;
	scanf("%d",&s);
	int ans=1.2*60*60/s;
	printf("%d",ans);
}
```
