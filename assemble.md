http://asm.sourceforge.net/articles/linasm.html

```
// push rbp ti stack
push   %rbp 
```

```
// LEA (load effective address)
// https://stackoverflow.com/questions/1658294/whats-the-purpose-of-the-lea-instruction
lea    -20(%rbp), %rax 
```

```
// move rsp to rbp
mov    %rsp, %rbp 
```

```
sub   $32, %rsp
```