# Symptoms
Using JUnit tests lets look at the outputs of the code and use it to determine which part of the method is not working as intended.

---
Here is our failure inducing test: \
\
![Image](lab3_bugs_1.png)	\
\
Here we can see that the actual output has the result of 11.0/3 instead of 11.0/2 (this is based on the numbers as a fraction 
rather than decimal). Based on the output we can assume that something is wrong with the removal of the lowest number(s) as 
the sum is the correct expected amount and the divisor is the issue.

---
Here is our non-failure inducing test: \
\
![Image](lab3_bugs_2.png) \
\
Here we see the code working as intended. Based on the above output we can assume that the code is at least taking out the lowest 
number for the sum and dividing, at least in this case, by the right number. Based on this info we compare and contrast
this to the previous test in order to determine the issue.

---
Based on this information lets look at the part of the method relating to the division and see if anything is wrong.
