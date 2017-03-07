# ARM体系结构与接口技术 第天

## 课程目的

1. 掌握 PWM
	* PWM 原理讲解
	* PWM 模块讲解
	* Exynos 4412 PWM 框图
	* Exynos 4412 PWM 寄存器介绍
	* Exynos 4412 PWM 示例代码分析
2. 掌握 RTC
	* RTC 模块讲解
	* Exynos 4412 RTC 框图
	* Exynos 4412 RTC 寄存器介绍
	* Exynos 4412 RTC 示例代码分析
3. 掌握 WDT
	* WDT 模块讲解
	* Exynos 4412 WDT 框图
	* Exynos 4412 WDT 寄存器介绍
	* Exynos 4412 WDT 示例代码分析

## 教学大纲

* 晶振，时钟，分频
* PWM 控制蜂鸣器
* RTC - 实时时钟(Real Time Clock)
* WDT - 监视定时器(Watch Dog Timer)

## 教学内容

* [PWM](PWM.md)
* [RTC](RTC.md)
* [WDT](WDT.md)

## 作业安排

1. 查阅 "Exynos 4412 User Manual" 手册中关于 Clock,PWM,RTC,WDT 相关章节
2. 阅读 光盘文件 "华清远见-CORTEXA9资料1.iso" 中的 "/使用手册/实验手册/ARM体系结构与接口技术FS4412.pdf"
3. 阅读,编译,运行,分析实验手册中相关代码
	* 3.Buzzer_PWM
	* 4.WDT_INT
	* 5.Alarm_RTC
	* 5.RTC