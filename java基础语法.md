# 笔记1：Java基础语法

## 一、Java历史

> 1.1991年sun公司Green项目
>
> 2.1999年java分成javaSE、javaEE、javaME
>
> 3.2009年甲骨文公司收购java

## 二、java学习

> Java核心优势：跨平台
>
> avaSE：定位在个人计算机上的应用
>
> JVM：Java虚拟机
>
> 是一种规范，就是一个虚拟的用于执行bytecode字节码的计算机。
>
> windows常用命令：
>
> dir：查看
>
> md：创建
>
> rd：删除
>
> cd：改变
>
> cmd默认的编码格式是gbk，在执行文件代码是可以改变文件的编码格式。
>
> jdk安装：在java运行时需要安装jdk
>
> jvm、jre、jdk 说明：
>
> jvm是java虚拟机  jre是java运行环境包含jvm   jdk java开发工具包包含jre
>
> 1. 类的创建
>
>    第一步新建文件 HelloWorld.java
>
>    第二步打开文件编写代码：
>
>    ```
>    public class  HelloWorld{
>      public static void main(String[] args){
>        System.out.println("HelloWorld!!!");
>      }
>    }
>    class Test{
>      
>    }
>    ```
>
>    第三步编译文件，在文件相应的目录下执行javac HelloWorld.java
>
>    第四步运行java程序，在相应目录下执行java  HelloWorld
>
>    注意：1、文件名和类名一致。
>
>    ​	    2、一个文件中可以有多个类名，但是public修饰的只有一个。
>
>    ​	    3、运行文件时需要main方法，它是所有java程序的入口
>
>    ​	    4、main方法的参数可以有不同的写法：String[]  args、String   []    args 、  String     args[]。
>
>    ​	    5、参数名字无所谓一般是args
>
>    ​	    6、每行的代码要以;结束。
>
>    ​	    7、java代码要使用{}括起来
>
>    注释的类型：
>
>    单行注释：//
>
>    多行注释：/*     */
>
>    文本注释： /**
>
>    ​		    *    每一行都有一个*
>
>    ​		    */
>
>    开发原则：
>
>    ​	缩进；
>
>    ​	成对（括号、引号等等）；
>
>    ​	见名知意；
>
>    标识符：
>
>    ​	作用：常量、变量、方法、类、包等名称。
>
>    ​	规范：
>
>    ​		1、字母、下划线、美元符号开头
>
>    ​		2、其他必须是字母、数字、下划线、美元符
>
>    ​		3、标识符大小写敏感
>
>    ​		4、不能是java的关键字和保留字
>
>    ​	常规：
>
>    ​		1、驼峰法则
>
>    ​			1）类名首字母大写
>
>    ​			2）方法变量首字母小写
>
>    ​			3）多个单词拼接每个单词的首字母大写
>
>    ​		2、见名知意：千万不要写拼音
>
>    关键字/保留字
>
>    ​	128个
>
>    ASCII 英文字符集 1个字节
>
>    ISO-8859-1 西欧字符集 1个字节
>
>    BIGS 台湾的 繁体汉字 2个字节
>
>    GBS2312 大量使用的最早的简体中文集 2字节
>
>    GBK    GBK2312扩展可以有繁体中文 2字节
>
>    ​	    GB18030  2字节
>
>    unicide 国际通用 2字节 
>
>
> 2、基本数据类型
>
> ​	java是强类型语言
>
> ​	常量是有数据类型的。
>
> ​	变量必须有数据类型修饰
>
> ​	基本数据类型 ：  4类8种
>
> ​					数值	整型：byte 、 short、int、long
>
> ​							浮点: float、double
>
> ​					字符	char
>
> ​					布尔	boolean
>
> ​				byte：1字节-128——127
>
> ​				short：2字节 -32768——32767
>
> ​				int：4字节   +-21亿 -2147483648到+-2147483648
>
> ​				long： 8字节		
>
> ​				float：4字节 -3.4E+38 和 3.4E+38
>
> ​				double：8字节-1.7E-308～1.7E+308
>
> ​				char：2字节
>
> ​				boolean： 1位 两个值
>
> 转义符：
>
> ​	\b 退格  \n 换行 \t 制表  \r 回车 \“  双引号
>
> ​	引用数据类型：
>
> ​		类、接口、数组
>
> ​	常量：值不会改变，Final 修饰
>
> ​	变量：值会改变。
>
> ​			先声明，后赋值
>
> ​			声明+赋值
>
> ​			给变量赋值过程中变量的值成为常量。
>
> ```
> public class Study01{
> 	// 单行  方法名首字母小写 
> 	/* 
> 		多行   类名首字母大写 
> 	
> 	*/
> 	/**
> 	* 文本 
> 	*/
> 	public static void main(String[] args){
> 		
> 		byte a = 1;
> 		System.out.println(a);
> 		short b= 144;
> 		System.out.println(b);
> 		int c = 123123123;
> 		System.out.println(c);
> 		long d = 456789999;
> 		System.out.println(d);
> 		char e = '我';
> 		System.out.println(e);
> 		boolean f = true;
> 		System.out.println(f);
> 		String g= new String("我是谁");
> 		System.out.println(g);
> 		
> 		
> 	}	
> 	
> }
> ```
>
> 运算符：
>
> ​	算术运算符： + - * / % ++ --
>
> ​	赋值运算符： =
>
> ​	扩展运算符： += -+ *= /=
>
> ​	关系运算符 ： > < >=  <=  ==  !=
>
> ​	逻辑运算符： && || ！
>
> ​	位运算符： &  | ^ ~ >>   << >>>
>
> ​	条件运算符： ？ ：	
>
> ```
> 逻辑运算符 && 表示短路与 两边表达是从左向右开始对比如果左边是fale右边不需要判断，两边有一个是false整体结果false
> ||  短路或  两边表达是从左向右开始对比如果左边是true右边不需要判断，两边有一个是true整体结果true
> 位运算符： &与  |或 ^异或 ~ 取反 >>移位   << >>>  在操作是会转换成二进制数进行运算
> ？：  1>2?2:3  结果是3  先判断如果是true 返回？后面的false 返回：后面的
> ```
>
> ​				

 