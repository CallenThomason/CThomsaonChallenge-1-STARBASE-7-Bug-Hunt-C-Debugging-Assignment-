# Bug Log

**Name:** ______________________

Fill in one row for every bug you find and fix in `Program.cs`. There are
**33 bugs**: 12 syntax, 5 runtime, 16 logic. Keep the rows in line-number order
if you can.

**Kind** must be one of: `Syntax`, `Runtime`, `Logic`.

The first row is a worked example of the level of detail expected (it is **not** one of the 33 bugs).

| # | Section | Line | Kind | What was wrong | How I fixed it |
1 | Section 1 | line 32 | Syntax | Missing an end quote inside the Write |Added the end quote |
2 | Section 1 | line 34 | Logic | Wanted to take the first later, but had a 1 for the index| changed the index from 1 to 0 |
3| Section 1 | line 35 | Runtime | crewName.Length is out of bounds for the index |added a -1 to get the last index |
4| Section 2 | line 56 | Syntax | Missing the '()' after .ReadLine |Added the paranthesis |
5| Section 2 | line 57 | logic | saving crewName as the age variable |Changed crewName to ageInput |
6| Section 2 | line 61 | Syntax | 18 inclusive |changed <= to <|
7| Section 2 | line 76 | logic | code only runs if someone is a commander and officer |changed && to || |
8| Section 3 | line 97 | Syntax | int is capitalized |changed Int to int |
9| Section 3 | line 104 | logic | attempts is not being incremented |changed attempts = 1 to attempts++ |
10 | Section 3 | line 106 | Syntax | uses the assignment operator for a comarison |changed = to == |
11| Section 4 | line 142 | Runtime error | <= callSign.Length is out of bounds |changed to < callSign.Length |
12| Section 4 | line 144 | logic | concatination is wrong |changed i + 1 to (i + 1) |
13| Section 5 | line 175 | logic | not adding all the levels to totalfuel |changed = to += |
14| Section 5 | line 185 | Syntax | mispelled totalFuel |changed totalFule to totalFuel|
15| Section 6 | line 202 | Syntax | missing statement terminator |added statment terminator |
16| Section 6 | line 206 | logic | adding price and total ordered as the subtotal |changed + to * |
17| Section 6 | line 209 | logic | mulipling by 0.10 which is actually division |changed 0.10 to 1.10 |
18| Section 6 | line 218 | Syntax | finalTotal + 5 is causing an error |changed + to += |
19| Section 7 | line 229 | logic | 1 is not included|changed > to >=  |
20| Section 7 | line 232 | logic | LIFTOFF is going to be printed after each iteration|moved it outside the for loop |
21| Section 8 | line 244 | syntax | while loop is missing()|added () |
22 | Section 9 | line 266 | syntax | used commas instead of statment terminator|changed , to ; |
23| Section 9 | line 266 | syntax | used commas instead of statment terminator|changed , to ; |
24| Section 10 | line 288 | syntax | using '' instead of ""|changed '' to ""|
25| Section 10 | line 290 | logic| odd inputs should print PORT side| changed the 1 to a 0|
26 | Section 10 | line 295 | Syntax| no closing curly brace|closed the curly brace|
27  | Section 11 | line 312 | logic | math for the leftover is wrong|changed to  rationCredits - (rationCredits / crewCount) * crewCount  ; |
28 | Section 12 | line 330 | logic| calls to crewName instead of clearance|changed crewName to |
29| Section 12 | line 333 | Syntax| line was lowercase in WriteLine()|corrected the casing|
30 | Section 8 | line 246 | RunTime| No end condition|added ping++|
31| Section 5 | line 167 | logic| decimal isn't being printed |changed totalFuel to a double|
32 | Section 5 | line 170 | logic| does not take 5 tanks |added <= 5 so it runs 5 times|
33  | Section 9 | line 267 | logic| is running rows number of times, should run row number of times |changed rows to row|
34 | Section 11 | line 312 | Runtime| math is done too early and divids by zero|changed the 0 to 1, assuming their is at least 1 crew memmber|
35 | Section 11 | line 314 | logic| computation is done before user inputs crewCount |moved computation to be done after crewCount is established by user.|

## Reflection (a few sentences)

Which bug took you the longest to find, and why?

The bug that took me the longest to solve was trying to print the average fuel number as a fraction. It took me the longest 
because it was a logic error. Their was no red line telling me where it was at. I wasn't sure what or where was going wrong.
Evertually I found that totalFuel also needed to be a double in order to output a decimal.  

Which kind of bug (syntax, runtime, logic) do you think is the hardest to catch? Why?
The most difficult kind of error to catch are logic errors. Their are no yellow or red lines telling you something is wrong. 
You just have to know the program isn't doing what you want it to do. Figuring that out comes from several bug tests. 
