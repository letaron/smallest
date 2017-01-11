# TINY
 gcc -Wall tiny.c
gcc -Wall -s tiny.c
gcc -Wall -s -O3 tiny.c
nasm -f elf64 tiny.asm && gcc -Wall -s tiny.o
after main -> _start  nasm -f elf64 tiny.asm && gcc -Wall -s -nostartfiles tiny.o
