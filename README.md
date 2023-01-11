# Compiler Final Project

## Files
* fin.l
* fin.y

## How to compile
fin is file name.
* bison -d -o fin.tab.c fin.y
* gcc -c -g -I.. fin.tab.c
* flex -o fin.yy.c fin.l
* gcc -c -g -I.. fin.yy.c
* gcc -o fin fin.tab.o fin.yy.o -ll

## How to test
example is test file name.
* ./fin ./smli < example.lsp
