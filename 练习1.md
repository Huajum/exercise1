# exercise1
初学1
#define _CRT_SECURE_NO_WARNINGS 1

//包含叫stdio.h的文件
//std- 标准 standard  input output
#include<stdio.h>
//井号#是指令形式

int num2 = 1;//全局变量


int main()//主函数-程序入口-main函数有且只有一个
{   
	//将test01的源文件 g_val用到这里
	//声明extern外部符号的
	extern int  g_val;
	printf(" g_val =%d\n", g_val);
	

	//输入2个数的和
	int num0 = 0; //  局部变量 一定在代码块内部（{}）
	int num1 = 0;
	int sum = 0;//C语言语法规定，变量定义在当前代码块的最前面
	
	//输入数据-使用输入函数scanf
	scanf("%d%d", &num0, &num1);//&取地址符号
	
	sum = num0 + num1;
	printf("sum=%d\n", sum);
	//这里完成任务
	//print fuction  -  printf  -打印函数
	//库函数 - C语言本身提供给我们使用的函数
	//井号#是指令形式，include
	printf("Hello world\n");

	char ch = 'a';//内存  char字符串类型
	printf("%c\n", ch);//%c - 打印字符格式的数据
	
	int age = 20;
	printf("%d\n",age);//%d -- 打印整型十进制数据
	
	float f= 5.0;
	printf("%f\n", f);

	double d = 3.14;
	printf("%lf\n",d);//lf 双精

	/////

	printf("%d\n", sizeof(char));
	printf("%d\n", sizeof(short));
	printf("%d\n", sizeof(int));
	printf("%d\n", sizeof(long));
	printf("%d\n", sizeof(long long));
	printf("%d\n", sizeof(float));
	printf("%d\n", sizeof(double));

	/// 
	////char - 字符类型
	////%c-打印字符 %d-打印整型 %f-打印浮点数  
	//// 依次推%f-  地址形式  x-16进制

	return 0;
}
  
//int 是整型的意思

//计算机单位
//  bit - 比特拉   2进制 0 1  为一个bit
//byte - 字节     1byte=  8bit =  2进制数1011011
// kb
// mb -兆b
// gb
// tb
// pb
// 

//字节跳动-抖音、西瓜视频是字节公司byte dance
//
//十进制  123 = 3*10^0+2*10^1+1*10*2
// 二进制   1100 = 1*2^3+1*2^2+0+0=9
//
// 1字节=8bit  2^3
// short int =2字节=16 
//即2进制
// 2^(16-1)=65535
//


//float 申请4个字节存放小数
//sizeof(long)>=sizeof(int)  long字节4或8
