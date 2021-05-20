## 第一題 三數最小 
```c
#include <stdio.h>
int abc(int a,int b,int c)
{
	int ans=a;
	if(ans>b)ans=b;
	if(ans>c)ans=c;
	return ans;
}
int main()
{
	int a,b,c;
	scanf("%d%d%d",&a,&b,&c);
	printf("%d\n",abc(a,b,c));
}
```

## 第二題 數字個數
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	n=n%10000;
	printf("%d",n/1000);
}
```

## 第三題 判斷平方數
```c
#include <stdio.h>
int main()
{
	int n,ans=0;
	scanf("%d",&n);
	for(int i=0;i<2000;i++)
	{
		if((i*i)==n)ans=i;
	}
	if(ans>0)printf("%d",ans);
	else printf("0");
}
```

## 第四題 計算質數個數
```c
#include <stdio.h>
int main()
{
	int a,b,ans=0,j;
	scanf("%d%d",&a,&b);
	for(int i=a;i<=b;i++)
	{
		for(j=2;j<i;j++)
		{
			if(i%j==0)
			break;
		}
	if(j==i)
	ans++;
	}
	printf("%d",ans);
}
```

## 第五題 三數組合 
```c
#include <stdio.h>
int main()
{
	int a[3],i,temp;
	for(i=0;i<3;i++)
	{
		scanf("%d",&a[i]);
	}
	for(int i=0;i<3;i++)
	{
		for(int j=i;j<3;j++)
		{
			if(a[i]<a[j])
			{
				temp=a[i];
				a[i]=a[j];
				a[j]=temp;
			}
		}
	
	}
	
		printf("%d",a[0]*100+a[1]*10+a[2]+1);
}
```
