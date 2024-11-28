# 实验三 分支结构程序设计
##一、实验目的 
1、了解C语言表示逻辑量的方法（以0代表“假”，以1代表“真”）。 
2、学会正确使用逻辑运算符和逻辑表达式。 
3、熟练掌握if语句和switch语句。 
4、熟悉分支结构程序设计。 
##二、实验准备 
1、复习关系、逻辑、条件运算符和表达式。 
2、复习if语句的三种形式。 
3、复习if语句的嵌套并能正确分析。 
4、复习多分支选择switch语句。
##三、实验内容
(1)、
#include<stdio.h>
int main(){
	int a,b,c,d;
	scanf("%d %d %d",&a,&b,&c);
   if(a>b){
       d=a;
       a=b;
       b=d;
   }
   if(a>c){
       d=a;
       a=c;
       c=d;
   }
   if(b>c){
       d=b;
       b=c;
       c=d;
   }
       printf("%d %d %d",a,b,c);
    return 0;

}
问题:该代码的作用是什么?
答案:比较三个数的大小并输出.
(2)、
#include<stdio.h>
int main(){
	int b;
	printf("请输入数字:");
	scanf("%d",&b);
	switch( b/10 ) {
	case 9:
		printf("good!");
		break;
	case 8:
		printf("good!!");
	    break;
	case 7:
	    printf("good!!!");    
	    break;
	default:
	    printf("try again");
		break;
	}
    return 0;
	}
 问:该代码的作用是什么?
这段 C 语言代码的主要功能是：提示用户输入一个整数，然后根据该整数除以 10 后的结果进行不同情况的输出判断。如果结果是 9、8、7 则分别输出不同程度的 “good” 字样，若结果是其他值则输出 “try again”。
