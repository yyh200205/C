# C
初学C语言
//指针
int main()
{
	int a = 10;
	int* p = &a;
	printf("%p\n", &a);
	printf("%p\n", p);
  printf("%p\n", &p);
  return 0;
}

//结构体
结构体变量：.
 结构体指针：->
结构体、指针
struct Book
{
	char name[20];
	int price;
};
int main()
{
	struct Book b1 = { "高等数学",20 };
	struct Book* pb = &b1;
	printf("书名：%s\n", pb->name);
	printf("书名：%s\n", ( * pb).name);
	printf("价格：%d\n", ( * pb).price);
	printf("%p\n", pb);
	printf("%p\n", &b1);
	printf("书名:%s\n", b1.name);
	printf("价格:%d元\n", b1.price);
	b1.price = 15;
	printf("修改后的价格:%d元\n", b1.price);
	return 0;
}

//分支语句
//是否为奇数
int main()
{
	int a = 0;
	while (a <= 100)
	{
		if (a % 2 == 1)
		{
			printf("%d\n", a);
			a++;
		}
		else
			a++;
	}
	return 0;
}
int main()
{
	int a = 0;
	printf("请输入a:");
	scanf_s("%d", &a);
	if (a % 2 == 1)
		printf("a是奇数\n");
	else
		printf("a不是奇数\n");
	return 0;
}
