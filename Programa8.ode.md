# Programa que pida dos números por puerto de entrada y devuelva el mayor por puerta de salida 

<reg>

PC:1000

</reg> 

<mem>

    1000: 4000  #IN r0,00 
    1001: 4100  #IN r1,00 
    1002: 2D08  #LLI rD,08 
    1003: 3D10  #LHI rD,10 
    1004: 7201  #SUBS r2 r0-r1
    1005: C200  #BR 2, salto si s=1
    1006: 5000  #OUT OP00, r0
    1007: F000  #HALT
    1008: 5100  #OUT OP00, r1
    1009: F000  #HALT

</mem>
