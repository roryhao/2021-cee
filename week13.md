## 第一題 求11 +22+33+…+nn
```c
#include <stdio.h>
int main()
{
	int n,ans=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i++)
	{
		ans+=i*10+i;
	}
	printf("%d",ans);
}
```

## 第二題 求兩數之最大公因數
```c
#include<iostream>
using namespace std;
int GCD(int a, int b)
{
	int ans=0;
	for(int i=1;i<=b;i++)
	{
		if(a%i==0 && b%i==0)
		ans=i;
	}
	return ans;
}
int main(){
  int a,b;cin>>a>>b;
  cout<<GCD(a,b)<<endl;
  return 0;
}
```

## 第三題 區間測速-超速之王 
```c
#include <stdio.h>
int main()
{
	int a,m,ans=1;
	scanf("%d",&m);
	for(int i=2;i<10;i++)
	{
		scanf("%d",&a);
		if(m>a)
		{
			m=a;
			ans=i;
		}
	}
	int s=60*60*1.2/m;
	printf("%d %d",ans,s);
}
```

## 第四題 10數排序，從大到小排好 
```c
#include <stdio.h>
int main()
{
	int a[10];
	for(int i=0;i<10;i++)
	{
		scanf("%d",&a[i]);
	}
	for(int j=0;j<10;j++)
	{
		for(int i=0;i<j;i++)
		{
			if(a[j]>a[i])
			{
				int t=a[j];
				a[j]=a[i];
				a[i]=t;
			}
		}
	}
	for(int i=0;i<10;i++)
	{
		printf("%d ",a[i]);
	}
}
```

## 第五題 正整數平方總和
```c
#include <stdio.h>
int main()
{
	int n,ans=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i++)
	{
		ans+=i*i;
	}
	printf("%d",ans);
}
```

## 第六題 兩數之間的3倍數總和 
```c
#include <stdio.h>
int main()
{
	int a,b,ans=0;
	scanf("%d%d",&a,&b);
	for(int i=a;i<=b;i++)
	{
		if(i%3==0)
		ans+=i;
	}
	printf("%d",ans);
}
```

## 第七題 判斷座標的象限 
```c
#include <stdio.h>
int main()
{
	int a,b;
	scanf("%d%d",&a,&b);
	if(a>0&&b>0)printf("1\n");
	if(a<0&&b>0)printf("2\n");
	if(a<0&&b<0)printf("3\n");
	if(a>0&&b<0)printf("4\n");
}
```

## 第八題 輸入n (n>0)， 求n之所有因數和
```c
#include <stdio.h>
int main()
{
	int n,ans=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i++)
	{
		if(n%i==0)
		ans+=i;
	}
	printf("%d",ans);
}
```
