# gcc - the GNU Compiler Collection

site : http://gcc.gnu.org/

gcc 是 GNU/linux 上的默认的C语言编译器。

## gcc 编译c语言源代码到可执行程序的四个步骤

1. 预编译(Pre-processing)

> `gcc -E hello.c -o hello.i`

2. 编译(Compiling)

> `gcc –S hello.i –o hello.s`

3. 汇编(Assembling)

> `gcc –c hello.s –o hello.o`

4. 链接(Link)

> `gcc hello.o other.o –o hello`