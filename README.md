DIVISION:
        INP 
        STA A
        INP
        STA B
        LDA 99
        STA C
LOOP    LDA A
        BRZ END
        LDA A
        SUB B
        STA A
        LDA C
        ADD Y
        STA C
        BRA LOOP
END     LDA C
        OUT C
        HLT
A       DAT
B       DAT
C       DAT
Y       DAT 1
