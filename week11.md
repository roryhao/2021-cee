## 第一題 字串中的數字個數
```c
#include <stdio.h>
char a[81];
int main()
{
	int b=0;
	scanf("%s",&a);
	int i=0;
	while(a[i]!='\0')
	{
		if('0'<=a[i]&&a[i]<='9')
		b++;
		i++;
	}
	printf("%d",b);
} 
```
  
## 第二題 利用自訂函式最大值max與最小值min求出兩者之差
```c
#include <stdio.h>
#include <iostream>
using namespace std;
int max(int a,int b,int c,int d)
{
	int x=a;
	if(x<b) x=b;
	if(x<c) x=c;
	if(x<d) x=d;
	return x;
}
int min(int a,int b,int c,int d)
{
	int x=a;
	if(x>b)x=b;
	if(x>c)x=c;
	if(x>d)x=d;
	return x;
}
int main()
{
  int a,b,c,d;cin>>a>>b>>c>>d;
  cout<<(max(a,b,c,d)-min(a,b,c,d));
  return 0;
}
/* 上方C++ main 函式 等同於 下方 C 的 main 函式
int main(void){
  int a, b, c, d;
  scanf("%d %d %d %d", &a, &b, &c, &d);
  printf("%d",  max(a,b,c,d) - min(a,b,c,d) );
  return 0;
}
*/
```
## 第三題 奇數之和
```c
#include <stdio.h>
int main()
{
	int n,ans=0;
	scanf("%d",&n);
	for(int i=1;i<=n;i+=2)
	{
		ans+=i;
	}
	printf("%d",ans);
}
```

## 第四題 兩數間可被7整除的數
```c
#include <stdio.h>
int main()
{
	int a,b;
	scanf("%d%d",&a,&b);
	for(int i=a;i<=b;i++)
	{
		if(i%7==0)
		printf("%d ",i);
	}
}
```
