# Beginners
2021.05
#include<stdio.h>
#include<string.h>
int main()
{
	int a = 10;
	int b = 20;
	int max = 0;
	max = (a > b ? a : b);
	printf("max=%d", max);
	return 0;
}
//int main()
//{
//	int a = 3;
//	int b = 5;
//	int c = a && b;// &&逻辑与 ||逻辑或
//	printf("c=%d\n", c);
//	return 0;
//}
//int main()
//{
//	int a = (int)3.14;//a=3
//	printf("a=%d\n", a);
//	return 0;
//}
//int main()
//{
//	int a = 10;
//	int b = a--;
//	printf("a=%d,b=%d", a, b);
//	return 0;
//}
//int main()
//{
//	int a = 1;
//	int b = ~a;
//	printf("%d\n", b);//b=-1 源码 反码 补码
//	return 0;
//}
//int main()
//{
//	int a = 10;
//	int arr[] = { 1,2,3,5,6,8,9 };
//	printf("%d\n", sizeof(a));
//	printf("%d\n", sizeof(int));//括号必须有
//	printf("%d\n", sizeof arr);
//	printf("%d\n", sizeof arr/sizeof arr[0]);//括号可有可无
//	return 0;
//}
//int Add(int x, int y)
//{
//	int z = x + y;
//	return z;
//}
//int main()
//{
//	int num1 = 10;
//	int num2 = 20;
//	int sum = 0;
//	sum = Add(num1, num2);
//	printf("sum=%d\n", sum);
//
//	return 0;
//}
//int main()
//{
//	int num1 = 0;
//	int num2 = 0;
//	int sum = 0;
//	printf("输入两个操作数:>");
//	scanf("%d,%d\n", &num1, &num2);
//	sum = num1 + num2;
//	printf("sum%d\n", sum);
//	return 0;
//}

//int Max(int x, int y)
//{
//	if (x > y)
//		return x;
//	else
//		return y;
//}
//int main()
//{
//	int num1 = 10;
//	int num2 = 20;
//	int max = 0;
//	max = Max(num1, num2);
//	printf("max=%d\n", max);
//	return 0;
//}
//int main()
//{
//	int num1 =10;
//	int num2 =11;
//	if (num1 > num2)
//		printf("请输出较大值%d\n", num1);
//	else
//		printf("请输出较大值%d\n", num2);
//	return 0;
//}
#include<stdio.h>
#include<string.h>
#define MAX(X,Y) (X>Y?X:Y)
int main()
{
	int a = 10;
	int b = 20;
	int max = MAX(a, b);
	printf("max=%d\n", max);
	return 0;

}
//extern int Add(int, int);
//int main()
//{
//	int a = 10;
//	int b = 20;
//	int sum = Add(a, b);
//		printf("sum=%d\n", sum);
//	return 0;
//}
//int main()
//{
//	extern int g_val;
//	printf("g_val=%d\n",g_val);
//	return 0;
//}
//void test()
//{
//	static int b = 1;
// static修饰局部变量
// 局部变量生命周期变长
// static修饰全局变量
// 改变了变量的作用域---让静态的全局变量只能在自己所在的源文件内部使用
// 出了源文件就没法使用
//	b++;
//printf("b=%d\n", b);
//}
//
//int main()
//{
//	int i = 0;
//	while (i < 5)
//	{
//		test();
//		i++;
//	}
//	return 0;
//}
//5.18
#include<stdio.h>
#include<string.h>
struct Book
{
	char name[20];
	short price;
	int designer;//int可输出  char不可
};
int main()
{
	struct Book b1 = { "C语言程序设计",55 ,"胥楚才"};
	struct Book* pb = &b1;
	printf("%s\n", (*pb).name);
	printf("%d\n", (*pb).price);
	printf("%s\n", (*pb).designer);//有点问题
	///*printf("书名:%s\n", b1.name);
	//printf("价格：%d元\n", b1.price);
	//b1.price = 15;
	//printf("修改后的价格：%d元\n",b1.price);*/
	return 0;
}
//int main()
//{
//	printf("%d\n", sizeof(int*));
//	printf("%d\n", sizeof(char*));
//	printf("%d\n", sizeof(short*));
//	printf("%d\n", sizeof(double*));
//	return 0;
//}
//int main()
//{
//	char ch = 'w';
//	char* pc = &ch;
//	*pc = 'T';
//	printf("%c\n", ch);
//	return 0;
//}
//int main()
//{
//	int a = 10;
//	int* p = &a;
//	printf("%p\n", p);
//	printf("%p\n", &a);
//	*p = 20;
//	printf("a=%d\n", a);
//	return 0;
//}
