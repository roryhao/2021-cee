## 第一題 億萬富翁
```c
#include <stdio.h>
#include <string.h>
int main()
{
	char a[100];
	scanf("%s",&a);
	for(int i=0;i<strlen(a);i++)
	{
		if((strlen(a)-i)%3==0 && i!=0)printf(",");
		printf("%c",a[i]);
	}
}
```

## 第二題 秒數換算  
```c
#include <stdio.h>
int main()
{
	int s;
	scanf("%d",&s);
	int a=s/60/60;
	if(a<10)printf("0%d:",a);
	else printf("%d:",a);
	
	int b=s/60%60;
	if(b<10)printf("0%d:",b);
	else printf("%d:",b);
	
	int c=s%60%60;
	if(c<10)printf("0%d",c);
	else printf("%d",c);
}
```
## 第三題 水杯接水
```c
#include <stdio.h>
int main()
{
	int n,m;
	scanf("%d%d",&n,&m);
	if(n/m==0)printf("%d",n/m);
	else
	printf("%d",n/m+1);
}
```

## 第四題 平面兩座標的面積
```c
#include <stdio.h>
int main()
{
	int X,Y,x,y,ans=0;
	scanf("%d%d%d%d",&X,&Y,&x,&y);
	ans=(x-X)*(y-Y);
	if(ans<0)ans=-ans;
	printf("%d",ans);
}
```

## 第五題 整數向量相加 
```c
#include <stdio.h>
int main()
{
	int n,a[10],b[10];
	scanf("%d",&n);
	for(int i=0;i<n;i++)
	{
		scanf("%d",&a[i]);
	}
	for(int i=0;i<n;i++)
	{
		scanf("%d",&b[i]);
		printf("%d ",a[i]+b[i]);
	}
}
```
