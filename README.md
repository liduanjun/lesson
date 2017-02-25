# 嵌入式课程笔记

[华清远见嵌入式课程大纲](http://www.embedu.org/courses/course/)

## 目录说明

1. 计算机语言
	* C语言
		* C语言基础课程(补习课程，不是正课)
		* C语言高级课程("Linux基础"放在这儿一起讲)
		* C语言的数据结构
	* C++语言
		* C++语言
2. Linux基础
3. Linux应用程序开发
	1. C语言
		* 普通应用程序开发
		* 网络应用程序开发
	2. C++语言
		* QT应用程序开发
4. Linux驱动程序开发
	* ARM体系结构和接口技术
	* 系统移植
	* 驱动程序开发
	* Android 底层
5. 项目实战
	* 仓储物联网管理系统

## 使用教程

* 此文档是由 git 来管理文件的，如果不清楚 git 的语法，建议查看[Git教程](5.项目/代码管理/Index.md)
* 此文档是由 Markdown 语法编写的，如果不清楚 Markdown 的语法，建议查看[Markdown教程](5.项目/代码管理/Index.md)

## 项目规范

* 每个文件夹下都有个 Index.md 文件，用于描述当前目录各个文件的作用。
* 每个文件夹下都有个 resouce 文件夹，用于存放除.md文件外的所有文件。
* .md 文件应该以 驼峰法 命名，即单词首字母大写，其余小写。
* .gitignore文件包含了本项目不想被包含进入git仓库的文件，比如c文件编译过程中生成的.o文件最终执行文件.bin文件
* 空的文件夹一般不会被git跟踪，你可以在空文件夹中创建一个 .gitkeep 文件来让此文件夹被跟踪
* .vscode 包含了默认的vscode编辑器的配置，你也可以选择其他编辑器开发此项目
* README.md 是此文件，是打开项目第一个被阅读的文件

