## 第十六週
## 第一題 大於漸增數列總和之最小整數 
```c
#include <stdio.h>
int main()
{
	int k,i,sum=0;
	scanf("%d",&k);
	for(i=1;i<k;i++)
	{
		sum+=i;
		if(sum>k)
		break;
	}
	printf("%d",i);
}
```

## 第二題 計算級數的值
```c
#include <stdio.h>
int main()
{
	int n,ans=0;
	scanf("%d",&n);
	for(int i=1;i<=(2*n+1);i+=2)
	{
		ans+=i;
	}
	printf("f(%d)=%d",n,ans);
}
```

## 第三題 拆解輸入的正整數 
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	int i=1;
	while(n>0)
	{
		printf("%d ",(n%10)*i);
		n/=10;
		i*=10;
	}
}
```

## 第四題 計算一組任意數目的整數的總和
```c
#include <stdio.h>
int main()
{
	int ans=0,n;
	scanf("%d",&n);
	while(n!=0)
	{
		if(n>0)
		ans+=n;
		scanf("%d",&n);
	}
	printf("%d",ans);
}
```

## 第五題 整數最大值、最小值 
```c
#include <stdio.h>
int main()
{
	int a,b,n;
	scanf("%d",&n);
	a=n;
	b=n;
	while(n!=0)
	{
		scanf("%d",&n);
		if(a>n)a=n;
		if(b<n)b=n;
	}
	printf("[%d,%d]",a,b);
}
```
