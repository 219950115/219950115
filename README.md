#include<stdio.h>
#include<string.h>
int main()
{
	char a[]=" ";
	printf("请输入想要查询的英文句子：\n");
	gets(a);
	int num=0;
	char *pa,*pb;
	int i;
	for (i=0;i<strlen(a);i++)
	{
		pa=&a[i];
		pb=&a[i+1];
		if(*pa=='it'&&*pa=='It')
		{
			num=num+1;
		}
	}
	printf("此句话it单词的个数为:%d\n",num);
 }
