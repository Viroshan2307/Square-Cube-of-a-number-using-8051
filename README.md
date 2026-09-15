# Square-Cube-of-a-number-using-8051
# 8051 Square  Program

## AIM
To write and execute an Assembly language program for finding the square of a given data using 8051 microcontroller in Keil software.

## APPARATUS REQUIRED
- Personal computer
- Keil μVision IDE

## ALGORITHM
1. Enter the Assembly language program.
2. Provide the input value to Port 0 (P0).
3. Execute the program.
4. The output square value is stored in Port 2 (P2).

## PROGRAM
```
ORG 0000H

MOV A, P0          ; Get input from Port 0
MOV B, A           ; Copy input to B
MUL AB             ; A × B = square

MOV P2, A          ; Store lower byte of square in P2

HERE: SJMP HERE

END









```

## OUTPUT
Input: 05H Square: 05H × 05H = 19H

P0 = 05H P2 = 19H

## RESULT
Thus, the square of the given data is calculated using 8051 Keil.

# 8051 Cube  Program

## AIM
To write and execute an Assembly language program for finding the cube of a given data using 8051 microcontroller in Keil software.

## APPARATUS REQUIRED
- Personal computer
- Keil μVision IDE

## ALGORITHM
1. Enter the Assembly language program.
2. Provide the input value.
3. Execute the program.
4. The output cube value is stored in a memory location.

## PROGRAM
```
ORG 0000H

MOV A, P0          ; Get input from Port 0
MOV B, A
MUL AB             ; A × A = square

MOV R2, A          ; Store lower byte of square
MOV R3, B          ; Store higher byte of square

MOV A, R2
MOV B, P0
MUL AB             ; Lower byte of square × input

MOV R4, A          ; Store lower byte of cube

MOV A, R3
MOV B, P0
MUL AB             ; Higher byte of square × input

MOV R5, A          ; Store middle byte of cube
MOV R6, B          ; Store higher byte of cube

HERE: SJMP HERE

END








```


## OUTPUT
OUTPUT

Input: 05H Cube: 05H × 05H × 05H = 7DH

P0 = 05H Cube = 00007DH

Output bytes:

R6 = 00H R5 = 00H R4 = 7DH
## RESULT
Thus, the cube of the given data is calculated using 8051 Keil.


