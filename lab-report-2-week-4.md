# Lab Report 2 - GitHub Changes from Week 4
Back to [All Labs](https://njmorales.github.io/cse15l-lab-reports/)

## Code Change 1: Fixing an infinite loop
* GitHub commit: 
![Image](codechange1.png)
* [Failure-inducing input file](testincorrect.md)
* Symptom input: 
![Image](symptom1input.png)
* Symptom output: 
![Image](symptom1output.png)
* The bug we found was that we did not check for the possibility of the nextOpenBracket having the value of -1 due to the fact that the "[" character was not found in the given substring from the markdown test file. This caused an infinite loop of reassigning variables to the same values, which we were able to detect because we inserted print statements in the code to track these values. Eventually, the code was updated to end the while loop and return if the values of any brackets or parentheses were -1. 