# 0x19. C - Stacks, Queues - LIFO, FIFO

## monty program description

A language interpreter made in the C programming language to manage stacks and queues (LIFO and FIFO). The aim is to interpret Monty bytecodes files. [Monty](http://montyscoconut.github.io/) is a language that aims to close the gap between scripting and programming languages.


## Compilation 

    gcc -Wall -Werror -Wextra -pedantic *.c -o monty

## Usage

    ./monty byte_file.m


## Allowable opcodes and what they do;
| opcode | functionality |
| --- | --- |
| push	| add element to the 'top' of stack and 'end' of queue. |
| pop	| remove element from 'top' of stack and 'end' of queue. |
| pall	| print every member of the structure. |
| pint	| prints the member value at the top of stack. |
| swap	| swaps the order of the 1st and 2nd elements in stack. |
| add	| add top two member values. |
| sub	| subtract the top element from the 2nd top element. |
| div	| divide the 2nd element by the top element. |
| mul	| multiply the top two elements of the stack. |
| mod	| the remainder when the 2nd element is divided by the top element. |
| comment	| there is the ability to parse comments found in bytecode ->'#'. | 
| pchar	| print character at the top of the stack. |
| pstr	| print the character at the top of the stack. | 
| rotl	| moves element at the top to the bottom of the stack. |
| rotr	| the bottom of the stack becomes the top. |
| queue, stack	| toggles the doubly link list implementation style. |
| nop	| opcode should do nothing. |

**Example:** **`$ cat opcodetestfile.m`**

`push 1`

`push 2`

`push 3`

`pall`

`$ ./montyfile opcodetestfile.m`

`3`

`2`

`1`

`$`

## Exit Status
Exits with status `EXIT_FAILURE`


## Author
- Kiguli Mark: <a href= "https://markbrlaise.github.io/"> Portfolio </a>

