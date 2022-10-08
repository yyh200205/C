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
