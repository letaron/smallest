# Smallest linux 64 bits binary in da world (WIP)

## Requirements

  - nasm
  - gcc


## Test

```sh
./a.out ; echo $?
# 42
wc -c a.out
```


```sh
gcc -Wall tiny.c
gcc -Wall -s tiny.c
gcc -Wall -s -O3 tiny.c
nasm -f elf64 tiny.asm && gcc -Wall -s tiny.o
nasm -f elf64 tiny_start.asm && gcc -Wall -s -nostartfiles tiny_start.o
``` 
