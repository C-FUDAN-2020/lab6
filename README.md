Lab 6
=====

     本节目标：
          1. switch语句的使用。
          2. 循环语句的使用。
          
获取及提交lab
-------
获取：通过 https://github.com/C-FUDAN-2020/lab6 获取。

提交物：将你完成目标1、目标2的源代码文件作为 lab6 的提交物。

提交：将提交物文档命名为学号_姓名 （如20302010000_王明），提交至超星学习通对应的作业中。

截止时间：北京时间 2020年10月25日 23:59:59

switch语句的使用
-------
switch语句的一般形式：

         switch(整形表达式)
        { 
           case 常量表达式1:  语句1;
           case 常量表达式2:  语句2;
            … 
           case 常量表达式n:  语句n;
           default:  语句n+1;
        }
        
 switch主要需要注意的方面有两个：

1、从哪进：表达式的值与case后的值相同则进入，case顺序不影响结果

2、从哪出：遇到break或整个switch结束（break以前是为了灵活，现在是累赘）

与if语句的不同：

if语句中若判断为真则只执行这个判断后的语句，执行完就跳出if语句，不会执行其他if语句；而switch语句不会在执行判断为真后的语句之后跳出循环，而是继续执行后面所有case语句。

在每一case语句之后增加break语句，使每一次执行之后均可跳出switch语句，从而避免输出不应有的结果。

最后：

1、case后的常量表达式不能相同；

2、case后的语句可以有多个且不用花括号括起来；

3、case和default子句的先后顺序可以先后变动，default子句可以省略不用；


请思考，如何使用switch语句实现根据不同的指令执行不同的语句块？（以下给出部分代码，结合lab5作业相关，请给出完整的可运行的代码）
    
        switch( )
      {
             case '' :
               printf("打印命令提示\n");
               break;
             case '' :
               printf("打印当前地图\n");
               break;
             case '' :
               printf("导入地图\n");
               break;
             case '':
               printf("保存地图\n");
               break;
             case 'F' :
               printf("进入地图设计模式\n");
               break;
             case '' :
               printf("退出地图设计模式\n");
               break;
             case '':
               printf("生成下一代生命\n");
               break;
             case '':
               printf("开始生命游戏\n");
               break;
              case '':
               printf("停止生命游戏\n");
               break;
             case '' :
               printf("退出游戏\n");
               break;
             default :
              printf("Invalid input\");
              break;
      }       
    
循环语句的使用
-------
首先，循环语句一共由3种，分别为while语句，do-while语句以及for语句。

一、while语句循环

格式为while（表达式）循环体只能是一个语句，循环体的次数由循环条件决定，其中上式的表达式也称循环条件表达式，当此表达式的值为真的时候循环体执行。
即：只要当循环表达式为真的时候（给定的条件成立），就执行循环体语句。While语句特点：先判断条件表达式，后执行循环体语句。
二，do···while语句 

1.先执行循环体系中的结构，然后再判断while括号中的表达式是否成立，为了让程序清晰，易读，建议把循环体用括号括起来。

2.执行过程；先执行循环体，然后再检查条件是否成立，若成立，则继续循环。

3.一般形式；do

循环体

while（表达式）

4.对比；while语句是先判断后循环，do while语句是先循环后判断。

三，for循环语句

1.一般形式为 for（表达式1，表达式2，表达式3）

表达式1；设置初始条件，仅仅执行一次，可以为0个，一个或多个。

表达式2；循环条件表达式，用来判断是否继续循环。

表达式3；循环的调整，即对循环变量的约束。

2.一般形式for（循环变量赋初值；循环条件；循环变量约束）。

各种循环语句可以相互嵌套，形成嵌套结构。

四，如果我们在执行循环的过程中，达到了目的的时候，想要取消这个循环体，那我们该这么办那，这时候终止循环语句诞生了。

1.提前终止循环体系——break语句

用法；与if语句相结合，即满足什么终止循环。

一般形式if（条件句）break

2.提前结束本次循环——continue语句

用法同break语句。

3.区别；break是对整个循环体系的终止，而continue仅仅是对本次循环的提前结束。

因此，我们学到了，整个循环系统的框架，当然了，随着我们技术的提高，我们将会发现循环语句的更多的应用。
