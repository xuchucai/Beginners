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
