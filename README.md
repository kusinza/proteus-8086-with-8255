# proteus-8086-with-8255 and motor control 
Interfacing 8255 with 8086 microprocessor 
to control the DC motor 

8086 SOURCE CODE;
CODE SEGMENT PUBLIC ‘CODE’
ASSUME CS: CODE
START:
MOVE DX, 0746H
MOVE AL, 82H
PORTB EQU 0742H
PORTA EQU 0740H
PORTC EQU 0744H
OUT DL, AL
STT:
MOV DX, PORT B; motor will rotate anti clock-wise.
IN AL, DX
MOV DX, PORT A; motor will rotate clock-wise.
OUT DX, AL
MOV DX, PORT C
MOV BL, AL
NOT AL
OUT DX, AL
JMP STT; this loops the programme
