# 第一題 迴文判斷 
```c
#include <stdio.h>
#include <string.h>

int main()
{	
	char a[4];
	int i;
	scanf("%s",&a);
	int len=strlen(a);
	for(i=0;i<(len/2);i++)
	{
		if(a[i]!=a[len-1-i])
		break;		
	}
	if(i==(len/2))printf("YES\n");
	else printf("NO\n");
}
```

# 第二題 函數反序排列數字 
```c
#include <stdio.h>
int f(int n)
{	
	int ans=0;
	while(n!=0)
	{
		ans=ans*10+n%10;
		n=n/10;
	}
	return ans;
}

int main()
{
	int n;
	scanf("%d",&n);
	printf("%d\n",f(n));
}
```

# 第三題 陣列找出現次數 
```c
#include <stdio.h>
int main()
{
	int a[10],n,ans=0;
	for(int i=0;i<10;i++)
	{
		scanf("%d",&a[i]);
		if(a[i]==0)break;
	}
	scanf("%d",&n);
	for(int i=0;i<10;i++)
	{
		if(a[i]==n)
		ans++;
	}
	printf("%d\n",ans);
}
```

# 第四題 判斷大小
```c
#include <stdio.h>
int f(int a,int b)
{
	if(a<b)	return -1;
	if(a==b)return 0;
	if(a>b) return 1;
}
int main()
{
    int a, b;
    scanf("%d %d", &a, &b);
    printf("%d",f(a,b));
    return 0;
}
```

# 第五題 計算一列整數的總和
```c
#include <stdio.h>
int main()
{
	int a[100],n=1,ans=0;
	for(int i=0;i<100;i++)
	{
		scanf("%d",&a[i]);
		if(a[i]==999)break;
		ans+=a[i];
		n++;
		
	}
	for(int i=0;i<n;i++)
	{
		printf("Enter an integer ( 999 to end ): \n");
		
	}
	printf("%The total is: %d",ans);
}
```



