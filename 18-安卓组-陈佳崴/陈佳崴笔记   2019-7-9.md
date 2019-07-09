## java的基本语句
---
1、java创建后要先输入```public static void main(string[]args){}```来创建主函数而后在方括号填写语句。

2、输出语句：`System.out.println()或System.out.print()；`其中`println`是输出后加换行符。且输出内容有多个变量时用加号隔开。

3、flaot、long型变量的输入时要加后缀F、L；double可不加后缀。

4、变量精度的排序是：boolean、short、int、float、doube、long。在类型转换时以精度高的为准。

5、对于十进制转换为其他进制可以使用：`System.out.println(Integer.toString(125))`语句，其中`toBinary`为二进制，`toOctalstring`为八进制,`toHexString`为十六进制。

6、将其他进制转换为十进制可以使用： `System.out.println("Integer.parseInt("00001509",16))`语句,其中字符串内为数字，`int`内为需转换的进制。

7、位运算符`&`：当两个**整形**变量的对应的为都为1时则运算后的变量该位数为1。

8、位运算符`|`:当两个**整形**变量的对应的有一个为1时则运算后的变量该位数为1。

9、按位或运算符`^`:当a、b两个数据的对应位相同时则运算后变量该位为1，否则为0；

10、函数重载语句格式：`public static [类型] [名称]{}`;

11、数组的两种初始化方法：直接用`char a[]={1,2,3}`或
```
char a[]=new char [3];
a[0]=1;a[1]=2;a[2]=3;
```

12、数组遍历的新语句:
```
int i=0;
char b[3]={1,2,3};
for(i:b)
{
  System.out.println(i);
    }
}
```
13、用jdk的cmd命令编译步骤：先用javac选择对应的java后缀文件生成.class文件，然后用Java命令打开改文件。