# C语言问题记录表

### enum 和 define重复定义问题?

```
/* Tokens.  */
#ifndef YYTOKENTYPE
# define YYTOKENTYPE
   /* Put the tokens into the symbol table, so that GDB and other debuggers
      know about them.  */
   enum yytokentype {
     NOUN = 258,
     PRONOUN = 259,
     VERB = 260,
     ADVERB = 261,
     ADJECTIVE = 262,
     PREPOSITION = 263,
     CONJUNCTION = 264
   };
#endif
/* Tokens.  */
#define NOUN 258
#define PRONOUN 259
#define VERB 260
#define ADVERB 261
#define ADJECTIVE 262
#define PREPOSITION 263
#define CONJUNCTION 264
```
enum 和 define 重复定义不冲突,define在与编译时就消失了。

### gcc 四步编译

1. 预处理，生成预编译文件（.文件）:Gcc –E hello.c –o hello.i

2. 编译，生成汇编代码（.s文件）:Gcc –S hello.i –o hello.s

3. 汇编，生成目标文件（.o文件）:Gcc –c hello.s –o hello.o

4. 链接，生成可执行文件:Gcc hello.o –o hello