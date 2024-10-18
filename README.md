# Estudo de comandos NASM
## primeiros comandos

* Programa "Hello World"

```Assembly

global _start

    section .text
    _start:
        mov rax, 1
        mov rdi, 1
        mov rsi, msg
        mov rdx, 13 
        syscall
        
        mov rax, 60
        mov rdi, rdi
        syscall

        section .data
        message:db    "Hello, World",10
    