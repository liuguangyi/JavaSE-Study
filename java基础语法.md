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
>    ​
>
> 