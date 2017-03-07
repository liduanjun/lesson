# NEON

## 什么是NEON

ARM® NEON™ 通用 SIMD 引擎可有效处理当前和将来的多媒体格式，从而改善用户体验。
NEON 技术可加速多媒体和信号处理算法（如视频编码/解码、2D/3D 图形、游戏、音频和语音处理、图像处理技术、电话和声音合成），其性能至少为 ARMv5 性能的 3 倍，为 ARMv6 SIMD 性能的 2 倍。

通过干净方式构建的 NEON 技术可无缝用于其本身的独立管道和寄存器文件。
NEON 技术是 ARM Cortex™-A 系列处理器的 128 位 SIMD（单指令，多数据）架构扩展，旨在为消费性多媒体应用程序提供灵活、强大的加速功能，从而显著改善用户体验。它具有 32 个寄存器，64 位宽（双倍视图为 16 个寄存器，128 位宽。）

Advanced SIMD (NEON)[edit]
The Advanced SIMD extension (aka NEON or "MPE" Media Processing Engine) is a combined 64- and 128-bit SIMD instruction set that provides standardized acceleration for media and signal processing applications. NEON is included in all Cortex-A8 devices but is optional in Cortex-A9 devices.[83] NEON can execute MP3 audio decoding on CPUs running at 10 MHz and can run the GSM adaptive multi-rate (AMR) speech codec at no more than 13 MHz. It features a comprehensive instruction set, separate register files and independent execution hardware.[84] NEON supports 8-, 16-, 32- and 64-bit integer and single-precision (32-bit) floating-point data and SIMD operations for handling audio and video processing as well as graphics and gaming processing. In NEON, the SIMD supports up to 16 operations at the same time. The NEON hardware shares the same floating-point registers as used in VFP. Devices such as the ARM Cortex-A8 and Cortex-A9 support 128-bit vectors but will execute with 64 bits at a time,[80] whereas newer Cortex-A15 devices can execute 128 bits at a time.

ProjectNe10 is ARM's first open source project (from its inception). The Ne10 library is a set of common, useful functions written in both NEON and C (for compatibility). The library was created to allow developers to use NEON optimisations without learning NEON but it also serves as a set of highly optimised NEON intrinsic and assembly code examples for common DSP, arithmetic and image processing routines. The code is available on GitHub.

## NEON 可以做什么

* 观看任意格式的任意视频
* 编辑和强化捕获的视频 – 视频稳定性
* 锯齿消除渲染和合成
* 游戏处理
* 快速处理几百万像素的照片
* 语音识别
* 强大的多通道高保真音频处理