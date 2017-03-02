# ARM体系结构与接口技术 第5天

## 课程目的

1. 掌握 GPIO
	* GPIO 模块讲解
	* Exynos 4412 GPIO 框图
	* Exynos 4412 GPIO 寄存器介绍
	* Exynos 4412 GPIO 示例代码分析
2. 掌握 ADC
	* ADC 模块讲解
	* Exynos 4412 ADC 框图
	* Exynos 4412 ADC 寄存器介绍
	* Exynos 4412 ADC 示例代码分析

## 教学大纲

* GPIO 输入输出控制
* GPIO 模拟时序，读取DS18B20温度模块数据
* GPIO 按键中断
* ADC 普通查询式读取转换结果的数模转换
* ADC 用中断方式查询结果的数模转换
... 
未完待续

## 教学内容

* [流水灯](LED.md)
* [按键中断](KeyInterrupt.md)

## 作业安排

1. 查阅 "Exynos 4412 User Manual" 手册中关于 GPIO,Interrupt,ADC 相关章节
2. 阅读 光盘文件 "华清远见-CORTEXA9资料1.iso" 中的 "/使用手册/实验手册/ARM体系结构与接口技术FS4412.pdf"
3. 阅读,编译,运行,分析实验手册中相关代码
	* 1.LED_GPIO
	* 14.temperature
	* 2.Ket_Int
	* 6.ADC
	* 7.ADC_INT