# 第一題 除惡務盡 
```c
#include <stdio.h>
int main()
{
	char a[100];
	scanf("%s",&a);
	int i=0;
	while (a[i]!='\0')
	{
		if(a[i]!='2')
		printf("%c",a[i]);
		i++;
	}
	printf("\n");
}
```

# 第二題 擲骰統計
```c
#include <stdio.h>
int main()
{
	char a[100],b[7]={0};
	scanf("%s",&a);
	
	int i=0;
	while (a[i]!='\0')
	{
		b[a[i]-'0']++;
		i++;
	}
	for(int i=1;i<=6;i++)
	{
	printf("%d:%d\n",i,b[i]);
	}

}
```

# 第三題 函數找整數的最大數字
```c
#include <stdio.h>
int max_digit(int n)
{
	int max;
	max=n%10;
	while(n>0)
	{
		if((n%10)>max)max=n%10;
		n/=10;
	}
	return max;
}
int main(void)
{
  int n;
  scanf("%d", &n);
  printf("[%d]", max_digit(n));
  return 0;
}
```

# 第四題 星星等腰三角 
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	for(int k=1;k<=n;k++)
	{
		for(int i=0;i<(n-k);i++)
		{
			printf(" ");
		}
		for(int i=0;i<(k*2-1);i++)
		{
			printf("*");
		}
	printf("\n");
	}
}
```

# 第五題 分開整數的每個數字 
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	printf("%d   ",n/10000);
	n=n%10000;
	printf("%d   ",n/1000);
	n=n%1000;
	printf("%d   ",n/100);
	n=n%100;
	printf("%d   ",n/10);
	n=n%10;
	printf("%d",n/1);
}
```

# 第六題 字元判別
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%c",&n);
	if('A'<=n && n<='Z')printf("U");
	else if(n>='a' && n<='z')printf("L");
	else if(n>='0' && n<='9')printf("D");
	else printf("O");
}
```

# 第七題 數字之首 
```c
#include <stdio.h>
int main()
{
	char n;
	scanf("%c",&n);
	printf("%c",n);
}
```

# 第八題 輸出從0到N的偶數
```c
#include <stdio.h>
int main()
{
	int n;
	scanf("%d",&n);
	for(int i=2;i<=n;i+=2)
	{
		 printf("%d ",i);
	}
}
```
