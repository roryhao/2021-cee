## 第一題 最大公因數
```c
#include <stdio.h>
int main()
{
	int a,b,ans=1;
	scanf("%d%d",&a,&b);
	for(int i=1;i<=a;i++)
	{
		if(a%i==0&&b%i==0)
		ans=i;
	}
	printf("Enter two integers: \n");
	printf("The greatest common divisor of %d and %d is %d\n",a,b,ans);
	
}
```

## 第二題 字串長度
```c
#include <stdio.h>
#include <string.h>
int main()
{
	char a[100],b[100];
	scanf("%s %s",&a,&b);
	int lena=strlen(a);
	int lenb=strlen(b);
	if(lena>lenb)printf("1");
	else if(lenb>lena)printf("-1");
	else{
	printf("%d",strcmp(a,b));}
}
```

## 第三題 函數判斷質數
```c
#include <stdio.h>
#include <iostream>
using namespace std;
int prime(int n)
{
	scanf("%d",&n);
	if(n==2)return 1;
	else if(n%2==0)return 0;
	else return 1;
}
int main(){
  int n;cin>>n;
  cout<<"["<<prime(n)<<"]";
  return 0;
}
```

## 第四題 判斷迴文
```c
#include <stdio.h>
#include <string.h>
int main()
{
	char a[80];
	int i;
	scanf("%s",&a);
	int QAQ=strlen(a);
	for(i=0;i<(QAQ/2);i++)
	{
		if(a[i]!=a[QAQ-1-i])
		break;
	}
	if(i==(QAQ/2))printf("YES");
	else printf("NO");
}
```
