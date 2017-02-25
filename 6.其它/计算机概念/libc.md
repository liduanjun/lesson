# libc 问题集合

### 头文件归属

> dpkg -S /usr/include/x86_64-linux-gnu/asm

```
linux-libc-dev:amd64: /usr/include/x86_64-linux-gnu/asm
```

> dpkg -S /usr/include/x86_64-linux-gnu/bits/

```
libc6-dev:amd64: /usr/include/x86_64-linux-gnu/bits
```

asm == asm-generic < bits < sys 后者调用前者