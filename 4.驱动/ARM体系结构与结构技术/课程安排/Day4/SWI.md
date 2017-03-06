# SWI - Software Interrupt(软中断)

## 软中断代码示例

```
.text
	myrest:
		b init
		nop
		b s_handle
		nop
		nop
		nop
		nop
		nop
		nop
		nop
		nop


	init:
		bl init_serial
		ldr r0,=a
		ldr r6,=w1
		mrs r0,cpsr
		bic r0,#0b11111
		mov r1,#0b10000
		orr r0,r0,r1
		msr cpsr,r0
		mov r7,#0x33
		svc 2
		nop
		nop
	s_handle:
		mov r9,#33
		mov pc,lr
	loop:
		b .
.end
```