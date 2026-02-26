# Arithmetic-operation-using-8086
# 8086 Assembly Language Programs for Arithmetic Operations

## AIM

To write and execute Assembly Language Programs to perform arithmetic operations for the 8086 microprocessor.

---

## APPARATUS REQUIRED

* Personal Computer with MASM Software

---

## 1. ADDITION

#### Algorithm

1. Initialize memory location in HL register.
2. Store 1st data.
3. Increment HL to enter 2nd data.
4. Move 2nd number to accumulator.
5. Decrement HL.
6. Add value in memory with accumulator.
7. Store result.
8. Stop.


## FLOW CHART
<img width="707" height="1024" alt="image" src="https://github.com/user-attachments/assets/b5a7062d-e294-47cd-9683-a40de25e82de" />


#### Program

```asm
CODE SEGMENT
ASSUME CS:CODE, DS:CODE
ORG 1000H
MOV CL,00H
MOV AX,1234H
MOV BX,1234H
ADD AX,BX
JNC L1
INC CL
L1:MOV SI,1200H
MOV [SI],AX
MOV [SI+2],CL
MOV AH,4CH
INT 21H
CODE ENDS
END

```

#### Output Table
<img width="991" height="405" alt="image" src="https://github.com/user-attachments/assets/9705708a-d9a4-403a-9e18-a4380ddd009b" />


#### Manual Calculations
<img width="923" height="311" alt="image" src="https://github.com/user-attachments/assets/eb306711-a743-4eb0-8b7d-20561d1e27b6" />


---

## OUTPUT IMAGE FROM MASM SOFTWARE
<img width="826" height="550" alt="image" src="https://github.com/user-attachments/assets/0eaf0133-a5dc-4c94-8210-3a169dc0e89b" />

## 2. SUBTRACTION

#### Algorithm

1. Initialize memory and store 1st data.
2. Increment to get 2nd data.
3. Move 2nd data to accumulator.
4. Subtract memory content.
5. Store result.

## FLOWCHART

<img width="578" height="797" alt="image" src="https://github.com/user-attachments/assets/564c3c7a-33ce-4a1c-8920-beb5c24b9b47" />


#### Program
```asm
code segment
assume cs:code,ds:code
org 1000h
mov AX,1234h
mov BX,1234h
sub AX,BX
jnc down
inc CL
down:mov SI,1200h
mov [sI],AX
mov [SI+2],CL
mov ah,4ch
int 21H
code ends
end

```


#### Output Table
<img width="1010" height="413" alt="image" src="https://github.com/user-attachments/assets/8e6c927c-3ffc-4e2b-96a7-2f26b4c38c1d" />


#### Manual Calculations

<img width="606" height="374" alt="image" src="https://github.com/user-attachments/assets/7727ce35-699a-4a72-a457-809a745fcce2" />

---


## OUTPUT SCREEN FROM MASM SOFTWARE
<img width="818" height="545" alt="image" src="https://github.com/user-attachments/assets/597c9b42-4099-4027-8536-434268d05985" />

## 3. MULTIPLICATION

#### Algorithm

1. Initialize memory and store operands.
2. Move operands to registers.
3. Multiply.
4. Store result.

##FLOWCHART

<img width="569" height="906" alt="image" src="https://github.com/user-attachments/assets/88be88ff-2896-4a88-b73d-84ccffd2fcf9" />



#### Program

```asm
code segment
assume cs:code,ds:code
org 1000h
MOV DX,0000H
mov AX,1234h
mov BX,1234h
mul BX
mov si,1200h
mov [si],ax
mov [si+02h],dx
mov ah,4ch
int 21h
code ends
end

```

#### Output Table
<img width="940" height="632" alt="image" src="https://github.com/user-attachments/assets/318c0813-f583-48fb-b6b8-6b5bcbb791d0" />


#### Manual Calculations

<img width="683" height="568" alt="image" src="https://github.com/user-attachments/assets/e6d68a6c-6994-4eb8-8d4d-ed2a2708a5bd" />

---

## OUTPUT SCREEN FROM MASM SOFTWARE
<img width="992" height="478" alt="image" src="https://github.com/user-attachments/assets/992d5d92-f390-45c3-90ef-c4486a926c4b" />

## 4. DIVISION

#### Algorithm

1. Load memory location of operands.
2. Perform division.
3. Store result.

   ## FLOWCHART
<img width="1065" height="802" alt="image" src="https://github.com/user-attachments/assets/25b4a483-0d42-494b-8639-1af3ea17191b" />


#### Program

```asm
CODE SEGMENT
ASSUME CS:CODE,DS:CODE
ORG 1000H
MOV DX,0000H
MOV AX,1234H
MOV BX,1234H
DIV BX
MOV SI,1200H
MOV [SI],AX
MOV [SI+02H],DX
MOV AH,4CH
INT 21H
CODE ENDS

```

#### Output Table
<img width="940" height="609" alt="image" src="https://github.com/user-attachments/assets/dc4e6836-ae72-4c68-b8a8-14a835dc3117" />



#### Manual Calculations

<img width="520" height="421" alt="image" src="https://github.com/user-attachments/assets/20197144-32d2-4420-9b70-9de9ccc0f987" />

---
## OUTPUT FROM MASM SOFTWARE
<img width="940" height="629" alt="image" src="https://github.com/user-attachments/assets/f63212d5-98ee-4da2-aabc-637beb28e57b" />



## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.

