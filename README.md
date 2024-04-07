# NAME:PRADEEP V
# REG NO:212223240119

### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

/* write all the steps invloved */

**PROGRAM**
```
module EXP05(din, a, b, c); 
input [0:7] din; 
output a,b,c; 
assign a= (din[4] | din[5] | din[6] | din[7]); 
assign b= (din[2] | din[3] | din[6] | din[7]);
assign c= (din[1] | din[3] | din[5] | din[7]);
endmodule
```



```
/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by: Pradeep V 
RegisterNumber:212223240119
*/
```

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
![318334089-9b77a222-13f5-4514-aeb1-5f582ec840ca](https://github.com/velupradeep/ENCODER8TO3DATAFLOW/assets/150329341/5919d482-9ae3-430d-bcbf-e2b79d4bd8de)

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
![318336190-9a06c4c4-347a-4aa7-8f5c-8ae5a5fe03a6](https://github.com/velupradeep/ENCODER8TO3DATAFLOW/assets/150329341/00861236-e124-40ef-98cd-eb5be3ad991e)

**RESULTS**
Thus, the implement Encoder 8 To 3 in Dataflow Modelling using verilog in Quartus software is successfully verified.



