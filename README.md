

## NAME : Jayagar.T
## REG.NO : 24901219
 # EXPERIMENT-3: HALF ADDER AND SUBTRACTOR
 Implementation-of-Half-Adder-and-Half Subtractor-circuit
# AIM:
 To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog
 programming.
# EQUIPMENTS REQURIED:
 Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.
# HALF ADDER:
 Half adder is a combinational circuit that performs simple addition of two binary numbers. The
 input variables designate the augend and addend bits; the output variables produce the sum and
 carry. It is necessary to specify two output variables because the result may consist of two binary
 digits.
 Sum = A’B+AB’ =A ⊕ B Carry = AB
Figure -01 HALF ADDER
# HALF SUBTRACTOR:
 The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It
 has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To
 perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three
 possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we
 have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the
 next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a
 minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor
 needs two outputs. One output generates the difference and will be designated by the symbol D.
 The second output, designated B for borrow, generates the binary signal that informs the next
 stage that a I has been borrowed.
 Diff = A’B+AB’ =A ⊕ B Borrow = A’B
 Figure -02 HALF Subtractor
# PROCEDURE:
 1. Type the program in Quartus software.
2. Compile and run the program.
 3. Generate the RTL schematic and save the logic diagram.
 4. Create nodes for inputs and outputs to generate the timing diagram.
 5. For different input combinations generate the timing diagram.
# PROGRAM:

#### module halfaddsub(a,b,sum,carry,difference,borrow);
#### input a,b;
#### output sum,carry,difference,borrow;
#### assign sum=a^b;
#### assign carry=a&b;
#### assign difference=a^b;
#### assign borrow=(~a)&b;
#### endmodule

 # TRUTH TABLE:
![WhatsApp Image 2024-11-11 at 08 24 42_78839ad3](https://github.com/user-attachments/assets/2865eccc-1e76-4fb9-9c50-3f65877bc9c4)
![WhatsApp Image 2024-11-11 at 08 25 01_a13cd495](https://github.com/user-attachments/assets/64b258b7-0482-47f4-a285-2c242f923eb6)

# RTL
 OUTPUT:
Thus design a half adder and half subtractor circuit and verified its truth table in Quartus using
 Verilog programming.
 ![Screenshot 2024-11-11 082116](https://github.com/user-attachments/assets/dd95ee47-6b08-408d-89cf-437f105dd9f7)

# OUTPUT WAVEFORM:
![Screenshot 2024-11-11 082324](https://github.com/user-attachments/assets/0125dbb1-a40a-4416-9e4f-30199df189fa)

# RESULT:
Thus design a half adder and half subtractor circuit and verified its truth table in Quartus using
 Verilog programming
