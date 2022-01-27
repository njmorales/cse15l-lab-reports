# Lab Report 2 - GitHub Changes from Week 4
Back to [All Labs](https://njmorales.github.io/cse15l-lab-reports/)

## Code Change 1: Fixing an infinite loop
* GitHub commit: 
![Image](codechange1.PNG)
* [Failure-inducing input file](testincorrect.md)
* Symptom input: 
![Image](symptom1input.PNG)
* Symptom output: 
![Image](symptom1output.PNG)
* The bug we found was that we did not check for the possibility of the nextOpenBracket having the value of -1 due to the fact that the "[" character was not found in the given substring from the markdown test file. This caused an infinite loop of reassigning variables to the same values, which we were able to detect because we inserted print statements in the code to track these values. Eventually, the code was updated to end the while loop and return if the values of any brackets or parentheses were -1. 

## Code Change 2: Fixing a syntax issue
* GitHub commit: 
![Image](codechange2.PNG)
* [Failure-inducing input file](testincorrect2.md)
* Symptom input and output: 
![Image](symptom2.PNG)
* The bug here was the fact that we did not account for the possibility of bracket characters being a part of the clickable text for the link. This meant that the wrong nextCloseBracket value was used in the code, causing the link to not be detected and making the outputted list empty even though we expected that link to be included in the list. To fix this temporarily, we changed the detection of "]" to the detection of"](" to ensure that the code was searching for a link within the parentheses right after the closed bracket character. 