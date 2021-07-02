# Cryptarithmetic-Problem

Aim -

To solve cryptarithmetic problem and to execute a program for a given problem. (SEND + MORE = MONEY)

Algorithm -

1. We have used Constraint programming, which is an optimization technique that emerged from the field of artificial intelligence.
2. It is characterized by two key ideas: To express the optimization problem at a high level to reveal its structure and to use constraints to reduce the search space by removing, from the15
variable domains, values that cannot appear in solutions.
3. To solve this problem, we use a greedy algorithm where we try to give values to each of the letters in an orderly fashion and checking with the constraints, try to find the required solution.
4. Another method would be to write an algorithm that checks for values carried forward but this approach looks to be more successful and efficient.

Calculations –

1. SEND + MORE = MONEY
  S E N D
+ M O R E
------------------
M O N E Y
------------------
• From Column 5, M=1, since it is the only carry-over possible from the sum of 2 single digit numbers in column 4.
• To produce a carry from column 4 to column 5 'S + M' is at least 9 so 'S=8or9' so 'S+M=9or10' & so 'O = 0 or 1'. But 'M=1', so 'O = 0'.
• If there is carry from Column 3 to 4 then 'E=9' & so 'N=0'. But 'O = 0' so there is no carry & 'S=9' & 'c3=0'.
• If there is no carry from column 2 to 3 then 'E=N' which is impossible, therefore there is carry & 'N=E+1' & 'c2=1'.16
• If there is carry from column 1 to 2 then 'N+R=E mod 10' & 'N=E+1' so 'E+1+R=E mod 10', so 'R=9' but 'S=9', so there must be carry from column 1 to 2. Therefore 'c1=1' & 
'R=8'.
• To carry 'c1=1' from column 1 to 2, we must have 'D+E=10+Y' as Y cannot be 0/1 so D+E is at least 12. As D is at most 7 & E is at least 5 (D cannot be 8 or 9 as it is already
assigned). N is at most 7 & 'N=E+1' so 'E=5or6'.
• If E were 6 & D+E at least 12 then D would be 7, but 'N=E+1' & N would also be 7 which is impossible. Therefore 'E=5' & 'N=6'. D+E is at least 12 so that we get 'D=7' & 'Y=2'.

SOLUTION:

  9 5 6 7
+ 1 0 8 5
-----------------
1 0 6 5 2
-----------------

VALUES:
S=9
E=5
N=6
D=7
M=1
O=0
R=8
Y=2
