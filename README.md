### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**:

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/Nishanth-018/ENCODER8TO3DATAFLOW/assets/149347651/45674571-2938-47e9-80a2-2ba1c32d5d51)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/Nishanth-018/ENCODER8TO3DATAFLOW/assets/149347651/439e8243-83b9-442c-b4ce-19807d40eb38)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/Nishanth-018/ENCODER8TO3DATAFLOW/assets/149347651/5ea81932-e448-4536-b73c-0bc62e45be0d)

Figure 02  Encoder 8 * 3

**Procedure**
```
1.Type the program in Quartus software.
2.Compile and run the program.
3.Generate the RTL schematic and save the logic diagram.
4.Create nodes for inputs and outputs to generate the timing diagram.
5.For different input combinations generate the timing diagram.
```
**PROGRAM**
```
/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 
module encoder_top(din, a, b, c); 
input [0:7] din; 
output a,b,c; 
assign a=din[4] | din[5] | din[6] | din[7]; 
assign b=din[2] | din[3] | din[6] | din[7];
assign c=din[2] | din[4] | din[6] | din[7];
endmodule

Developed by: MOHAMED RIDWAN A
RegisterNumber: 212223110030
*/
```
## RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling
![image](https://github.com/Nishanth-018/ENCODER8TO3DATAFLOW/assets/149347651/91b7aecb-c256-446f-a2f6-6771674fa05c)

## TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling
![image](https://github.com/Nishanth-018/ENCODER8TO3DATAFLOW/assets/149347651/10fed669-656a-4ae9-beea-b396ee82bbc4)

## RESULTS
Thus the code is ececuted successfully.




