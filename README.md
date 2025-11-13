4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```
module Exp3(A, B,C,D,W,X,Y,Z,F1,F2);
input A, B, C,D,W,X,Y,Z;
wire w1,w2,w3,w4,w5,w6,w7,w8,w9,w10;
output F1,F2;
assign w1=(~A)&(~B)&(~C)&(~D);
assign w2=(A)&(~C)&(~D);
assign w3=(~B)&(C)&(~D);
assign w4=(~A)&(B)&(C)&(D);
assign w5=(B)&(~C)&(D);
assign w6=(X)&(~Y)&(Z);
assign w7=(~X)&(~Y)&(Z);
assign w8=(~W)&(X)&(Y);
assign w9=(W)&(~X)&(Y);
assign w10=(W)&(X)&(Y);
assign F1=w1|w2|w3|w4|w5;
assign F2=w6|w7|w8|w9|w10;
endmodule 
```
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: R NARESH KUMAR
RegisterNumber:212224040213




**RTL**
<img width="967" height="883" alt="de2" src="https://github.com/user-attachments/assets/451e9480-af8c-4808-9c4d-578f706ac7c4" />
![de22](https://github.com/user-attachments/assets/72e60d33-4f37-4f7f-88f9-9cbb22e8a310)


**Output:**
<img width="1624" height="767" alt="image" src="https://github.com/user-attachments/assets/ac519789-bc7a-42ce-860a-49cbbfe327dc" />



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

