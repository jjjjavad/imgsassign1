f# imgdsassign1
this is a binary language that operates on a 4 by 4 grid to draw some stuff
each word is 4bits
each instruction is 2 words
Address (First 4 bits): Where to move the cursor
Action (Second 4 bits): What to draw at that location
addresses
****0000,"(0,0)",Top Left
0001,"(0,1)",
0010,"(0,2)",
0011,"(0,3)",Top Right
0100,"(1,0)",Row 2 Starts
...,...,
1111,"(3,3)",Bottom Right**
actions
Binary,Shape,Description
**0000,     ,Erase (Empty)
0001,■,Solid Box
0010,X,Cross
0011,/,Forward Slash
0100,\,Back Slash
0101,O,Circle
1111,!,Error/Alert**
example  this code will draw an L shape using boxes
1. 0000 0001
2. 0100 0001
3. 1000 0001
4. 1001 0001

■
■
■  ■

now see if can draw a cross
