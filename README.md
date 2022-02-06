**SuperCPU BASIC**

Access your SCPU RAM from BASIC

To activate:

LOAD"SCPUBASIC",8,1

SYS49152

Commands:

@Bx  (x = sets the RAM bank number between 0 and 255)

@P addr,val  (just like POKE command, but using the current bank above)

Because this is a simple wedge, I couldnt implement a PEEK function, so instead I
took advantage of the USR() function.  To peek a value of the current bank:

x = USR(addr)

Enjoy

