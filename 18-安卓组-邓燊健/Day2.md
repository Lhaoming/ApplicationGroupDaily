## Day2 
### 一、Java语言的环境搭建
1、下载JRE   // JRE：Java Runtime Environment (Java 运行环境)  
JRE包括Java虚拟机（JVM  Java Virtual Machine）和Java 程序所需的核心类库等  
2、下载JDK   // JDK：Java Development Kit（Java 开发工具包）
JDK是提供给开发人员使用的，其中包含了Java的开发工具，也包含了JRE  
//简单理解：使用JDK开发完成的Java程序，交给JRE去运行  
3、配置环境变量  
4、验证是否成功  
### 二、Java程序开发体验——Hello World  
1、将Java代码编写扩展名为 .Java的文件中   //XXX.java 成为源文件  
2、通过Javac命令对该Java文件进行编译     //编译后，生成可执行的Class文件（或者成字节码文件）  
3、通过Java命令对生成的Class文件进行运行  
//编译使用的工具 Javac  运行工具 Java  
基本代码：  

	public static void main(String[] args) 
              {
		    // TODO Auto-generated method stub
		     System.out.println("Hello World！");
	        	}
/* 
步骤：  
1、	通过class关键字定义一个类，将代码都编写到该类中  
2、为保证该类的独立运行，在类中定义一个主函数，格式为：public static void main(String[] args)  
3、保存成一个拓展名为.java的文件  
4、在DOS控制台通过Javac工具对Java文件进行编译，生成一个class文件  
5、在DOS控制台通过Java工具对生成的class文件进行执行  
*/  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/DC4A2AB05B624C25BDE0409A28468A15/467)  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/9D01F9B6B064462CAB2B0200C063AD92/469)
### 三、Java中基础
1、注释  
① 单行注释   //努力学习Java语言  
② 多行注释   
③ 文档注释   /**   作者：XXX  版本：12.3*/  
注释作用：  
1、注解说明程序  
2、调试程序  
2、Java语言基础组成  
①关键字：被赋予特殊含义的词（必须小写）  
②标识符：在程序中自定义的一些名称  
组成：26个英文大小写字母、数字、下划线    
//注意：   
1、	标识符不可以以数字开头  
2、	不能使用关键字作为标识符    
③注释  
④常量和变量
常量：表示不能改变的数值（整数常量 6、小数常量1.3、布尔型常量true、字符常量’a’、字符串常量”A”、null常量）  
//对于整数：Java有三种形式：十进制、八进制（0开头）、十六进制（0X开头）  
//8个二进制数表示一个字节、若干个字节组成数据  
3个二进制位是一个八进制    
4个二进制位就是一个十六进制位
### 四、进制的转换
1、十进制转换成二进制：对十进制数进行除2取余（java中的System.out.println(Integer.toBinaryString(十进制数X))）  
2、二进制转化成十进制：二进制乘以2的过程  
3、负数的二进制形式：正数的二进制形式取反再加1的二进制形式（负数的最高位二进制都是1）  
变量：将不确定的数据进行存储，也就是在内存中开辟一个空间
