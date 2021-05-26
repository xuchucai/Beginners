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
#include<stdio.h>
#include<string.h>
#include<windows.h>
int main()
{
	int i = 0;
	char password[20] = { 0 };
	for (i = 0; i <3; i++)
	{
		printf("请输入密码\n");
		scanf("%s", password);
		if (strcmp(password, "tongyu1998") == 0)
		{
			printf("登陆成功\n");
			break;
		}
		else
		{
			printf("密码错误，请重新输入\n");
		}
	}
	if (i == 3)
	{
		printf("三次登陆失败，请找回密码\n");
	}
	return 0;
}
//int main()
//{
//	char arr1[] = "welcome to my heart";
//	char arr2[] = "###################";
//	int left = 0;
//	int right = strlen(arr1) - 1;
//	while (left <= right)
//	{
//		arr2[left] = arr1[left];
//		arr2[right] = arr1[right];
//		printf("%s\n", arr2);
//		Sleep(1000);
//		system("cls");
//		left++;
//		right--;
//	}
//	printf("%s\n", arr2);
//	return 0;
//}
//int main()
//{
//	int arr[] = { 1,2,3,4,5,6,8,9,10,11 };
//	int k = 1;
//	int sz = sizeof(arr) / sizeof(arr[0]);
//	int left = 0;
//	int right = sz - 1;
//	while (left <= right)
//	{
//		int mid = (left + right) / 2;
//		if (arr[mid] > k)
//		{
//			right = mid - 1;
//		}
//		else if (arr[mid] < k)
//		{
//			left = mid + 1;
//		}
//		else
//		{
//			printf("找到了，下标是：%d\n", mid);
//			break;
//		}
//	}
//	if (left > right)
//	{
//		printf("找不到\n");
//	}
//	return 0;
//}
//int main()
//{
//	int arr[] = { 0,1,2,3,6,11,12,13,23,24,30,77 };
//	int sz = sizeof(arr) / sizeof(arr[0]);
//	int left = 0;
//	int right = sz - 1;
//	int k = 12;
//	int mid = (left + right) / 2;
//
//		if (arr[mid] > k)
//		{
//			right = mid - 1;
//		}
//		else if (arr[mid] < k)
//		{
//			left = mid + 1;
//		}
//		else
//		{
//			printf("找到了，下标是： %d", mid);
//		}
//	 return 0;
//}
//int main()
//{
//	int arr[] = { 1,2,3,4,5,6,7,8,9,10 };
//	int k = 17;
//	int i = 0;
//	int se = sizeof(arr) / sizeof(arr[0]);
//	for (i = 0; i < se; i++)
//	{
//		if (k == arr[i])
//		{
//			printf("找到了，下标是：%d\n", i);
//			break;
//		}
//	}
//	if (i == se)
//		printf("找不到\n");
//	return 0;
//}
//int main()
//{
//	int n, i,M ;
//	int ret = 0;
//	for (n = 1; n <= 5; n++)
//	{
//		for (i = 1, M = 1; i <= n; i++)
//		{
//			M = i * M;
//		}
//		ret = ret + M;
//	}
//	printf("ret=%d\n", ret);
//	return 0;
//}
//int main()
//{
//	int i = 1;
//	do
//	{
//		printf("%d \n", i);
//		i++;
//	} 
//	while (i <= 10);
//	return 0;
//
//}
//int main()
//{
//	int x, y;
//	for (x = 0, y = 0; x < 2 || y < 5; ++x, y++)
//	{
//		printf("hehe\n" );
//	}
//		return 0;
//}
//int main()
//{
//	int i = 0;
//	int k = 0;
//	for (i = 0, k = 0; k = 0; i++, k++)
//	{
//		k++;
//	}
//	return 0;
//}
//int main()
//{
//	int j = 0;
//	int i = 0;
//	for (i=0; i < 10; i++)
//	{
//		for (j=0; j < 10; j++)
//		{
//			printf("%d\n",i*j);
//		}
//	}
//	return 0;
//
//}
//int main()
//{
//	int i = 0;
//	for (i = 1; i <= 10; i++)
//	{
//		if (5 == i)
//			continue;
//		printf("%d\n", i);
//	}
//		return 0;
//}
//int main()
//{
//	int ch = 0;
//	while ((ch=getchar()) != EOF)
//	{
//		if (ch < '0' || ch>'9')
//			continue;
//		putchar(ch);
//	}
//	return 0;
//
//}
//int main()
//{
//	int ret = 0;
//	int ch = 0;
//	int password[20] = { 0 };
//	printf("请输入密码:>");
//	scanf("%s", password);
//	while ((ret = getchar()) !='\n')
//	{
//		;
//	}
//	printf("请输入(Y/N):>");
//	ch = getchar();
//	if (ch == 'Y')
//	{
//		printf("确认成功\n");
//	}
//	else if (ch == 'N')
//	{
//		printf("取消确认\n");
//	}
//	else
//		printf("确认失败\n");
//
//
//	return 0;
//}
//int main()
//{
//	int ch = 0;
//	while ((ch = getchar()) != EOF)
//	{
//		putchar(ch);
//	}
//	return 0;
//}
//int main()
//{
//	int i = 1;
//	while (i < 11)
//	{
//		if (i == 5)
//			continue;
//		printf("%d\n", i);
//		i++;
//	}
//	return 0;
//}
//int main()
//{
//	int i = 0;
//	int a = 1;
//	while (i < 10)
//	{
//		a++;
//		i++;
//	}
//	printf("a= %d i= %d", a, i);
//	return 0;
//}
//int main()
//{
//	int n = 1;
//	int m = 2;
//	switch (n)
//	{
//	case 1:
//		m++;
//	case 2:
//		n++;
//	case 3:
//		switch (n)
//		{
//		case 1:
//			n++;
//		case 2:
//			n++;
//			m++;
//			break;
//		}
//	case 4:
//		m++;
//		break;
//	default:
//		break;
//
//	}
//	printf("m= %d n= %d\n", m, n);
//	return 0;
//}
//int main()
//{
//	int day = 0;
//	scanf("%d", &day);
//	switch (day)
//	{
//	case 1:
//		printf("星期一\n");
//		break;
//	case 2:
//		printf("星期二\n");
//		break;
//	case 3:
//		
//		printf("星期三\n");
//		break;
//	case 4:
//		printf("星期四\n");
//		break;
//	case 5:
//		printf("星期五\n");
//		break;
//	case 6:
//		printf("星期六\n");
//		break;
//	case 7:
//		printf("星期天\n");
//		break;
//	default:
//		printf("输入错误\n");
//		break;
//
//	}
//	return 0;
//}
//int main()
//{
//	int a = 1;
//	while (a <= 100)
//	{
//		printf("%d ", a);
//		a +=2;
//	}
//	return 0;
//}
//int main()
//{
//	int a = 1;
//	while (a <= 100)
//	{
//		if (a % 2 == 1)
//			printf("%d ", a);
//		a++;
//
//
//	}
//	return 0;
//}

	
//int main()
//{
//	int a = 0;
//	int b = 1;
//	if (a == 1)
//	{
//		if (b = 2)
//			printf("hehe\n");
//	}
//		else
//			printf("haha\n");
//	return 0;
//
//}
//int main()
//{
//	int age = 0;
//	scanf("%d", &age);
//	if (age < 18)
//	{
//		printf("未成年\n");
//	}
//	else if(age>=18 &&age<30)
//	{
//		printf("青年\n");
//	}
//	else if (age >= 30 && age < 55)
//	{
//		printf("壮年\n");
//	}
//	else
//	{
//		printf("老年\n");
//	}
//	return 0;
//}
//struct Stu
//{
//	char name[8];//多少个字节
//	int age;
//	char sex[5];
//	char ID[100];
//
//};
//int main()
//{
//	struct Stu s = { "胥楚才", 22,"男","2018" };
//	struct Stu* ps = &s;
//	printf("%s\n", ps->name);
//	printf("%d\n", (*ps).age );
//	printf("%s\n", (*ps).sex);
//	printf("%s\n", (*ps).ID);
//	printf("name=%s,age=%d,sex=%s,ID=%s\n", s.name,s.age , s.sex, s.ID);
//	printf("name=%s,age=%d,sex=%s,ID=%s\n", ps->name, ps->age, ps->sex, ps->ID);
//	printf("%d\n", sizeof(ps->name));
//	//printf("%d\n", sizeof name/sizeof name[0]);
//	return 0;
//}
//struct Book
//{
//	char name[20];
//	int price;
//	char designer[];//int可输出  char不可
//};
//int main()
//{
//	struct Book b1 = { "C语言程序设计",55 ,"胥楚才"};
//	struct Book *pb = &b1;
//	printf("%s\n", pb->designer);
//	///*printf("%s\n", (*pb).name);
//	//printf("%d\n", (*pb).price);
//	//printf("%s\n", (*pb).designer);*///有点问题
//	///*printf("书名:%s\n", b1.name);
//	//printf("价格：%d元\n", b1.price);
//	//b1.price = 15;
//	//printf("修改后的价格：%d元\n",b1.price);*/
//	return 0;
//}
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
