# Ex.No: 7  Logic Programming –  Logic Circuit Design
### DATE: 19/3/2024                                                                         
### REGISTER NUMBER : 212221040020
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
```
and(0,0,0).
and(0,1,0).
and(1,0,0).
and(1,1,1).
xor(0,0,0).
xor(0,1,1).
xor(1,0,1).
xor(1,1,0).
not(0,1).
not(1,0).
halfadder(A,B,Sum,Carry):-
    xor(A,B,Sum),
    and(A,B,Carry).
halfsub(A,B,Diff,Bor):-
    xor(A,B,Diff),
    not(A,X),
    and(X,B,Bor).

```



### Output:
![image](https://github.com/AshikaJubi/AI_Lab_2023-24/assets/129098066/94f18755-2e91-4562-b254-53047e607ec5)

![image](https://github.com/AshikaJubi/AI_Lab_2023-24/assets/129098066/a818e9dd-5585-43bb-89c6-49fe15a00243)




### Result:
Thus the truth table of circuit verified sucessfully.
