# 第一題 讀入整數反序列印
```c
#include <stdio.h>
int main()
{
	int a[10],n=0;
	for(int i=0;i<10;i++)
	{
		scanf("%d",&a[i]);
		if(a[i]==0)
		break;
		n++;
	}
	for(int i=n-1;i>=0;i--)
	{
		printf("%d ",a[i]);
	}
	printf("\n");
}
```
# 第二題 A的B次方函數
```c
#include <stdio.h>
int MYPOWER(int a,int b)
{
	int ans=1;
	for(int i=1;i<=b;i++)
	{
		ans=ans*a;
	}
	return ans;
}
int main(void)
{
	int a,b;
	scanf("%d%d",&a,&b);
	printf("[%d]",MYPOWER(a,b));
	return 0;
}

```
# 第三題 漸增數列相加 
```c
#include <stdio.h>
int main()
{
	int a,ans=0;
	scanf("%d",&a);
	for(int i=a;i>=2;i--)
	{
		
		ans+=(i-1)*i;
	}
	printf("%d\n",ans);
}
```
# 第四題 判別正方形 
```c
#include <stdio.h>
int main()
{
	int a,b;
	scanf("%d%d",&a,&b);
	if(a==b)printf("Enter two numbers:  It is a square ");
	else printf("Enter two numbers:  It is not a square ");
}
```
# 第五題 2進位轉10進位
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	int ans=0;
	ans=(n%10)*1;
	n=n/10;
	ans=(n%10)*2+ans;
	n=n/10;
	ans=(n%10)*4+ans;
	n=n/10;
	ans=(n%10)*8+ans;
	n=n/10;
	printf("%d\n",ans); 
}
```
# 第六題 均標與前標計算
```c
#include <stdio.h>
int main()
{
	int  n,a[100],sum=0,sumt=0,x=0;
	float avg,avgt;
	scanf("%d",&n);
	for(int i=0;i<n;i++)
	{
		scanf("%d",&a[i]);
	}
	for(int i=0;i<n;i++)
	{
		sum+=a[i];
	}
	avg=(float)sum/n;
	printf("均標:%.1f\n",avg);
	
	for(int i=0;i<n;i++)
	{
		if(a[i]>=avg)
		{
			sumt+=a[i];
			x++;
		}
	}
	avgt=(float)sumt/x;
	printf("前標:%.1f\n",avgt);
}
```
