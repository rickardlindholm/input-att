# input-att
att assembly handler x64

To run: gcc -o handler handler.s Mprov64.s 

To debug: gdb handler

Commands:
break inimage
run
step
next
info registers (examine all registers except for stackponters which contains addresses.

print/x $rax
d for decimal form, x for hexadecimal, t for binary form and c for ASCII

To check a register continouusly:
display $rax (to remove undisplay)

To check ascii & 12 byte 16, 32 is also possible, &inbuff equals the address of the "variable" inbuff.
x/12cb &inbuff
