# 第一題 反敘數字
```c
#include <stdio.h>

int main()
{	
	int n,ans=0;
	scanf("%d",&n);
	int temp=n;
	while(n!=0)
	{
		ans=ans*10+n%10;
		n=n/10;
	}
	printf("%d+%d=%d\n",temp,ans,ans+temp);
}
```
# 第二題 絕對值函數
```c
#include <stdio.h>
int f(int n)
{
	if(n<0)
	return n=-n;
	else
	return n;
}
int main(void)
{
	int n;
	scanf("%d",&n);
	printf("[%d]",f(n));
	return 0;
}
```

# 第三題 N數之和
```c
#include <stdio.h>
int main()
{
	int n,a,ans=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i++)
	{
		scanf("%d",&a);
		ans+=a;

	}
		printf("%d\n",ans);

}
```

# 第四題 三數極大
```c
#include <stdio.h>
int main()
{
	int a,b,c,max;
	scanf("%d%d%d",&a,&b,&c);
	if(a>b && a>c)max=a;
	else if(a<b && b>c)max=b;
	else max=c;
	printf("%d\n",max);
}
```
