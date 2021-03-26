# 第一題 計算陣列的平方值 
```C
#include <stdio.h>
int main()
{
	int a[100],N;
	scanf("%d",&N);
	for(int i=0;i<N;i++)
	{
		scanf("%d",&a[i]);
		printf("%d,",a[i]*a[i]);
	}
	printf("\n");
	
}

```

# 第二題 大小寫轉換 
```C
#include <stdio.h>
int main()
{
	char a[10];
	scanf("%s",&a);
	int i=0;
	while(a[i]!='\0')
	{
	if('A'<=a[i] && a[i]<='Z')
	printf("%c",a[i]-'A'+'a');
	else if('a'<=a[i] && a[i]<='z')
	printf("%c",a[i]-'a'+'A');
	else
	printf("%c",a[i]);
	i++;
	}
	printf("\n");
}
```

# 第三題 計算幾週與幾天
```C
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	printf("%d %d\n",n/7,n%7);
}
```

# 第四題 計程車資計算
```C
#include <stdio.h>
int main()
{
	int n,ans=1;
	scanf("%d",&n);
	if(n<2000)printf("100\n");
	if(n>2000)
	ans=(n-2000)/500;
	printf("%d\n",100+(5*ans)+5);
}
```

# 第五題 兩數間可被5整除的整數 
```C
#include <stdio.h>
int main()
{
	int a,b;
	scanf("%d%d",&a,&b);
	if(a<b)
	for(int i=a;i<=b;i++)
	{
		if(i%5==0)
		printf("%d\n",i);		
	}
	else if(a>b)
	for(int i=b;i<=a;i++)
	{
		if(i%5==0)
		printf("%d\n",i);
	}	
}
```

# 第六題 整數間最大距離
```C
#include <stdio.h>
int main()
{
	int a[3],max,min;
	for(int i=0;i<3;i++)
	{
		scanf("%d",&a[i]);
		min=a[0];
		max=a[0];
	}
	for(int i=0;i<3;i++)
	{
		if(min>a[i]) min=a[i];
		if(max<a[i]) max=a[i];

	}
		printf("%d\n",max-min);
}
```
