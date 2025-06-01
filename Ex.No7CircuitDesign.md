# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE:  1/4/2025                                                                         
### REGISTER NUMBER : 212222060112
### AIM: 
To write a logic program to design a circuit like half adder and half subtractor.
###  Algorithm:
1. Start the Program
2. Design a AND gate logic if both inputs are 1 then output is 1.
3. Design a OR gate logic if any one of input is 1 then output is 1.
4. Design a XOR gate logic if both inputs are different then output is 1.
5. Design a NOT gate logic if input is 0 then output is 1.
6. Design a half adder and half subtractor using the rules.
7. Test the logic.
8. Stop the program.

### Program:

% Half Adder
halfadder(X, Y, Sum, Carry) :-  
    xor(X, Y, Sum),  
    and(X, Y, Carry).  

% Half Subtractor
halfsubtractor(X, Y, Difference, Borrow) :-  
    xor(X, Y, Difference),  
    not(X, NA),  
    and(NA, Y, Borrow).  

% AND Gate
and(0, 0, 0).  
and(0, 1, 0).  
and(1, 0, 0).  
and(1, 1, 1).  

% XOR Gate
xor(0, 0, 0).  
xor(0, 1, 1).  
xor(1, 0, 1).  
xor(1, 1, 0).  

% NOT Gate
not(0, 1).  
not(1, 0).



### Output:
![image](https://github.com/user-attachments/assets/20a08e17-9687-457e-81e3-577f10b96759)




### Result:
Thus the truth table of circuit verified sucessfully.
