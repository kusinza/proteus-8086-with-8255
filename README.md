# proteus-8086-with-8255
Interfacing 8255 with 8086 microprocessor 

8255 PROGRAMMABLE PHERIPHERAL INTERFACE.
The Intel 8255A is a general purpose programmable I/O device designed for use
with Intel microprocessors. It consists of three 8-bit bidirectional I/O ports (24 I/O
lines) that can be configured to meet different system I/O needs. The three ports
are designated as PORT A, PORT B and PORT C. Port A contains one 8-bit output
latch/buffer and one 8-bit input buffer. Port B is same as PORT A or PORT B.
However, PORT C is split into two parts- PORT C lower (PC3-PC0) and PORT C
upper (PC7-PC4) by the control word. The four ports – two 8-bit PORTs and two 4
bit PORTs are divided in two groups Group A (PORT A and upper PORT C) Group B
(PORT B and lower PORT C) for programming purpose. These two groups can be
programmed in three different modes:. Mode-0, Mode-1 and Mode-2.
In the first mode, mode-0, each group may be programmed in either input
mode or output mode (PORT A, PORT B, PORT C lower, PORT C upper). In mode-1,
the second mode, each group may be programmed to have 8-lines of input or
output (PORT A or PORT B) and of the remaining 4-lines (PORT C lower or PORT C
upper) 3lines are used for handshaking and interrupt control signals. The third
mode of operation, mode-2, is a bidirectional bus mode which uses 8lines (PORT
A) only for a bidirectional bus and five lines (PORT C upper 4 lines and borrowing
one line from PORT C lower) for handshaking and control signals. PORT A and
PORT B have both input and output buffers and latches but PORT C has output
latch and input buffer.
