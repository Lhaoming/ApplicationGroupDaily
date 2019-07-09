## Day1

### 一、Git的基本简介
1、Git:一个开源分布式版本控制系统，可以有效、高速的处理从很小到非常大的项目版本管理。  
2、Git 是 Linus Torvalds 为了帮助管理 Linux 内核开发而开发的一个开放源码的版本控制软件。
（用C语言编写）   
3、适用系统：Linux、macOS、Solaris、Windows、Raspberry Pi
### 二、GIt的基本使用
#### 1、设置用户名和邮箱作为标识  
代码：  
$  git  config  --global  user.name "DSJLAQ"  //设置Git的用户名  
$  git config  --global  user.name  1623598270@qq.com  // 设置Git的用户邮箱  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/33690862E1514C25B896D08C6B26332D/270)
注意：git config --global 参数，有了这些参数，表明这台机器上所有的GIt仓库都会使用这个配置，也可以对某个仓库使用指定的用户名和邮箱。  
#### 2、创建一个版本库(repository)  
版本库也叫仓库，可以理解为一个目录，这个目录中的所有文件都可以被Git管理起来，每个文件的修改、删除，Git都可以进行跟踪。  
代码（D盘中Fighiting文件夹下创建一个名为Study的版本库）：  
$   cd D:  
$   cd Fighting  
$   cd  Study  
$   pwd     //pwd:命令是用于显示当前的目录  
$   git  init   //把这个目录变成git可以管理的仓库  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/86F21AB98E94490AA5E80C5B6281D414/281)  
通过以上的操作后，这时Study目录就会多一个 .git的目录，这个目录是用来跟踪管理版本的。  
#### 3、往版本库中添加文件（test.txt)  
代码：  
$ git add test.txt //使用 git add  文件名.文件类型  将文件添加到暂存区处  
$ git commit -m "test.txt文件已提交"  //使用 git commit -m "提交的注释" 把文件提交到版本库  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/D815FB8290CB428C8F7EEDB0FB1A19D8/310)  
出现了以上图片的内容说明，文件已经上传成功！  
#### 4、对文件进行修改（暂时没有上传到版本库中）  
$ git status  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/DB28D3D9CE504ADB8D5F92570A25D9CF/317)
代码：$ git  diff //查看修改后的文件差异  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/08A787C9D562455592215B289B746DB5/331)
#### 5、文件保存到版本库中  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/7FB7B53913D647E18324EFB7EE2CFB7E/342)  
#### 6、查看文件被修改的历史记录  
代码：$ git log  //也可以使用  $  git log --pretty=oneline(方便查看)  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/73749968F3BD4712808FA4F82AD89086/352)  
#### 7、版本还原（返回到上一个版本）  
代码：  
$ git reset --hard head^  //返回上一步的操作  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/E2225135C0394CD58B420B94986E1D20/380)
$ cat test.txt  //查看文件操作  
![image](http://note.youdao.com/yws/public/resource/ad4fc9c0144435fffff31abef2eded3a/xmlnote/37BFCAADE801431986855F55B96B548F/384)  
### 三、Java的初步认识
##### 1、什么是软件：  
一系列按照特定顺序组织的计算机数据和指令的集合  
##### 2、系统软件：  
DOS、Windows、Linux、MacOS等  
##### 3、应用软件：  
微信、QQ、WPS等  
##### 4、什么是开发：  
制作软件（软件的出现实现了人与计算机之间的更好的交互）  
##### 5、交互方式：  
①图形化界面：这种方式简单直观，使用者容易接受，容易上手操作  
②命令行方式：需要有一个控制台，输入指定的指令，让计算机完成一些操作。较为麻烦需要记住一些命令  
**Dos命令行，常见的命令**  
dir :列出当前目录下的文件以及文件夹  
md :创建目录  
rd :删除目录  
cd :进入指定目录  
cd.. :退出到上一级目录  
cd/ :退回到根目录  
del :删除文件  
exit :退出dos命令行  
##### 6、Java语言的概述：  
是SUN（standford Unvierstiy Network）斯坦福大学网络公司1995年推出的一门高级编程语言  
特点：  
①面向Internet的编程语言  
②Web应用程序的首选开发语言  
③完全面向对象、安全可靠、与平台无关的编程语言  
④跨平台性：通过Java语言编写的应用程序在不同的系统平台上都可以运行（原理： 操作系统具有一个Java虚拟机（JVM Java Virtual Machine）注意：虚拟机需要分系统：Windows系统、Linux系统、Mac系统等）  
##### 7、Java语言的三种技术架构  
①J2EE（Java 2 Platform Enterprise Edition）企业版：是为开发企业环境下的应用程序提供的一套解决方案，技术体系中包含技术如  Serviet Jsp等主要针对Web应用程序开发  
②J2SE（Java 2 Platform Standard Edition ） 标准版：是为开发普通桌面和商务应用程序提供解决方案（该技术是其他两者的基础）（Java版的扫雷）  
③J2ME（Java 2 Platform Micro Edition）小型版：是为开发电子消费产品和嵌入式设备提供的解决方案（手机中的应用程序）  

