- 👋 Hi, I’m @WANGZIXUANNB
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
WANGZIXUANNB/WANGZIXUANNB is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
#define _CRT_SECURE_NO_WARNINGS 1
#include<stdio.h>
//1.认识 注释：Ctrl+k+c
//int main()
//{
//	printf("hehe\n");
//    return 0;
//}  输入语句
//int main()
//{
//2.数据类型
//    char ch = 'a';
//    printf("%c\n",ch);  %c打印字符格式数据（非数字）
//	return 0;
//}  查打印字符数据（内存）
//int main()
//{
//	long num = 100;
//    printf("%d\n", num);  %d打印整型十进制(数字 )
//	return 0;
//}  打印各类数据的灵活运用
//int main()
//{ 
//	int num1 = 0;
//	int num2 = 0;
//	int sum =0;
//	scanf("%d%d",&num1,&num2);  scanf输入函数 &取地址
//	sum = num1 + num2;
//    printf("sum =%d\n",sum);
//	return 0;
//} 简易加减法计算机
//3.变量
//int global = 2020;
//
//int test()  可以用void代替int。 （因过于落后通常不建议。）
//{
//	printf("test - %d\n", global);gobal是字面常量，仅供自己使用，不是关键字。
//}
//int main()
//{
//	
//	printf("%d\n",global);
//	return 0;
//}  全局变量作用域展示
//4.常量（不包括#define）
//int main()
//{
//    const int num = 4;  const常量 作用 省空间 增加安全性 有常属性，但无法在条件仅限于常量数时使用，（本质是变量）
//    printf("%d\n",num);
//	return 0;
//}
//enum Color  枚举常量的应用
//{
//	RED,
//	YELLOW,
//	BLUE,
//};  如你所见 enum可以依次叠加数值 更安全方便
//int main()
//{
//    enum Color color = BLUE;
//    return 0;
//}
//5.字符串
//int main()
//{
//	char arr1[] = "abc";                这里的"abc" 实质为 'a','b','c','\0'
//	char arr2[] ={'a','b','c'};           改正 char arr2[] = {'a','b','c','\0'}; 或 = {'a','b','c',0};
//	printf("%s\n",arr1);
//    printf("%s\n",arr2);
//	return 0;
//}	  
//注意 这里会出来  abc
//                 abc乱码
//6.转义字符
//int main()
//{
//	printf("%d\n",strlen("c:\test\32\test.c")) ;  strlen定位后加位置
//    return 0;
//}  得出答案单位是bit 查内存
//ps:求数组个数 printf("%d\n",sizeof(arr)/sizeof(arr[0]));   数组字节总数/数组第一个元素的字节数量
//8.选择语句
//int main()
//{ 
//	int input = 0;
//	printf("欢迎\n");
//	printf("好好学习?(1/0)>");
//	scanf("%d",&input);
//	if(input == 1)
//	{
//	     printf("offer\n");
//	}
//	else; 注意 else是非法的没有适当的if与其匹配
//	{
//	    printf("打工\n");
//	}
//	return 0;
//}  //简易选择题  

//int MAX(int x,int y)
//{
//    if(x>y)
//       return x;
//	else
//	   return y;
//}
//int main()
//{
//    int num1 = 10;
//	int num2 = 20;
//	int max = 0;
//	max = MAX(num1,num2);
//	printf("max = %d\n",max);
//	return 0;  
//}  如何用MAX查大小（函数）
//9.循环语句
//int main()
//{
//	int line = 0;
//	printf("加入\n");
//	while(line<200)  
//	{
//	printf("敲\n");   改进：printf("敲：%d\n",line);可以为其增加编号。
//	line++;
//	}
//  if(line >= 200)   
//    printf("好offer\n");
//	return 0；
//}  循环输入 敲 直到200行 出现 好offer
//10.函数
//int add(int x,int y)  注意空格
//{
//    int z = x + y;
//		return z;
//}
//int main()
//{
//    int num1 = 0;
//	int num2 = 0;
//	int sum = 0;
//	printf("2,2:>"); 输入数值
//	scanf("%d%d",&num1,&num2);输入函数（位置）
//	sum = add(num1,num2);
//	return 0;
//}
//11.数组
//int arr{10} = {0,1,2,3,4,5,6,7,8,9};含义:定义一个整型数组最多放十个元素
//12.操作符
//int main()
//{
//	int a = 0;                    a:0 0 0 。。。 0
//	int b = ~a;                   b：1 1 1 。。。1     b：首位 为1 为负数 视为补码
//	printf("%d\n",b);               详解：  printf打印的是原码 
//	return 0;                         转换顺序 原码 1变0或0变1 成负码 末尾1变0或0变1 成补码  相反转换矣然  本题是 补变原
//}  得到的结果：-1               
//int main()
//{
//    int a = 10;
//    int b = a++;  含义:先使用，让b = a 。后++，使a：10 + 1 =11
//	printf("a = %d,b = %d\n",a,b);  
//	return 0;
//}  后置操作符   （前置同理）
//int main()
//{
//    int a = 3;
//    int b = 5;
//	int c = a && b;
//    printf("c = %d\n",c);  &&：逻辑与 类似并集 ||：逻辑或 类似交集
//	return 0;
//}  逻辑操作符   这题结果是1（为真命题，皆存在），若为0则反之
//int main()
//{
//    int a = 10;
//    int b = 20;
//	int max = 0;
//	max = (a>b?a:b);   格式:exp1?exp2：exp3   如果1不对，触发3.如果1对，触发2.
//	if(a>b)
//		max=a;
//	else
//		max=b;
//	return 0;
//}  条件操作符  
//int test()
//{
//    int a = 1;
//	a++;   a++ ：a=1+1=2  生成后不二次使用 ++a则反之
//	printf("a = %d\n",a);
//}
//int main()
//{
//    int i = 0;
//	while(i<5)
//	{
//		test();
//		i++;
//	}
//	return 0;
//}  简易计算机循环计算
//extern int Add(int,int);
//
//int main(）
//{
//    int a = 10;
//    int b = 20;
//	int sum = Add(a,b);
//	printf("sum=%\n",sum);
//	return 0;
//}  代码不完善
//14.#define
//#define MAX(x,y)(x>y?x:y)
//int main()
//{
//    int a = 10;
//    int b = 20;
//	int max = MAX(a,b);  在定义宏的影响下，实为 max = (a>b?a:b)
//	printf("max = %d\n,");
//	return 0;
//}  定义宏
//15.指针
//int main()
//{
//     int a = 10;
//	 int *p = &a;  
//     *p = 20;   故此时a=20
//	 
//}
//int main()
//{
//    double d = 3.14;
//	double *pd = &d;
//	*pd = 5.5;
//	printf("if\n",d);
//	printf("if\n",*pd);     %if:打印浮点数字小数
//}
//16.结构体
//struct book 
//{
//      char name [20];
//	  short price;
//};
//int main()
//{
//	struct book b1={"c",10};
//	printf("钢铁是怎么炼成的:%s\n",b1.name);
//	printf("10：%d\n",b1.price);
//	return 0;
//}   书名：钢铁是怎么炼成的
//      价格：10
//struct Book
//{
//       char name [20];
//	   short price;
//};
//int main()
//{
//	struct Book b1 = {"c语言程序设计",55};
//	struct Book *pb = &b1;
//	printf("%s\n",(*pb).name);
//	printf("%d\n",(*pb).price);
//	return 0;
//}   找书代码
