# FACTORIAL-OF-A-NUMBER-USING-8051-KEIL

**AIM:**

To write and execute Assembly language Program to perform factorial of a number using 8051 keil.
APPARATUS REQUIRED: Personal computer with Keil software

**ALGORITHM:**

• Start  

• Input: Read the number n.  

• Initialize:  

•Set factorial to 1.  

•Set i to 1.  

• Loop: While i is less than or equal to n:  

•Multiply factorial by i.  

•Increment i by 1.  

• Output: Store or print the value of factorial.  

• End

**FLOW CHART:**


<img width="261" height="308" alt="image" src="https://github.com/user-attachments/assets/bffe89f6-3ba9-4294-b817-8b545f680e66" />





**Program:**

ORG 0000H

MOV DPTR,#4500H

MOVX A,@DPTR

MOV R0,A

INC DPTR

ACALL FACTORIAL

MOVX @DPTR,A 

SJMP THIN 

FACTORIAL: DEC R0

CJNE R0,#01H,PRODUCT

SJMP THICK 

PRODUCT: MOV B,R0

MUL AB

ACALL FACTORIAL

THICK: RET 

THIN: RET

END

**Output:**  
![WhatsApp Image 2025-11-11 at 19 16 01_4129d41d](https://github.com/user-attachments/assets/3f15eae6-867f-4c2b-9703-e33c8bd07d5e)


**Manual Calculations:**  

![WhatsApp Image 2025-11-11 at 19 17 58_e023454e](https://github.com/user-attachments/assets/914ae9a0-9f50-4083-84d1-cbbffbbc8fc1)






**Result:**

Thus the factorial of a number using 8051 keil was calculated and shown the output.
