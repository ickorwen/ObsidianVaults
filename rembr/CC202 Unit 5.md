#West 
### Flowchart
- diagram that depicts a process, system or computer algorithm.
- When to Use a Flowchart?:
	-   To develop understanding of how a process is done  
	-  To study a process for improvement  
	-  To communicate to others how a process is done  
	-  When better communication is needed between people involved with the same process  
	-  To document a process  
	-  When planning a project  
	
		- Rectangle Shape - Represents a process
		- Oval or Pill Shape - Represents the start or end
		- Diamond Shape - Represents a decision
		- Parallelogram - Represents input/output

### While Looping

- statement can be simple or compound  

- expression acts as a decision maker and is usually a logical expression  
- statement is called the body of the loop

- i - loop control variable(LCV)

- infinite loop - continues to execute endlessly

- Counter-controleed while loop - 
	- When you know exactly how many times the statements need to be executed

- Sentinel-controlled - 
	- Loop ends when sentinel is encountered

- Flag-controlled while loop - 
	- uses a bool variable to control the loop  

- End-of-file (EOF)-controlled while loop: 
	- when it is  difficult to select a sentinel value 
	- The logical value returned by cin can determine if there is no more input
	

### for Looping
- called a counted or indexed for loop

- for (initial statement; loop condition; update statement)
	- statement

- The initial statement , loop condition, and update statement are called for loop control statements

- If the loop condition is initially **false**, the loop  
- body does not execute

- The update expression, when executed, changes the value of the loop control variable (initialized by the initial expression), which should change in such a way that eventuallysets the value of the loop condition to **false.**  
- The for loop body executes indefinitely if the loop condition is always **true**.

- you can omit all three statements, 2 semicolons still required


### do...while Looping
- do
	- statement
- while (expression);
- The statement executes first, and then the expression is evaluated
- To avoid an infinite loop, body must contain a statement that makes the expression false
- The statement can be simple or compound  
- Loop always iterates at least once

- ==Pretest loops== - loop condition evaluated before execution of body; while and for loops
- ==Posttest loops== - loop condition evaluated after execution of body; do... while
- always executes statement at least once

- can be used for input validation

All three loops have their place in C++  
– If you know or can determine in advance the number of  
repetitions needed, the for loop is the correct choice  
– If you do not know and cannot determine in advance the  
number of repetitions needed, and it could be zero, use a  
while loop  
– If you do not know and cannot determine in advance the  
number of repetitions needed, and it is at least one, use a  
do...while loop  


### break and continue statements

- alter flow of control
- break
	- exit early from loop
	- skip remainder of a switch structure

- continue
	- skips remaining statements and proceed with the next iteration of the loop

- nested loop
	- loop in a loop
	- ineer loop executed for each iteration of outer loop

### Avoiding Bugs by Avoiding Patches
- Software patch 
	- Piece of code written on top of an existing piece of code  
	- Intended to fix a bug in the original code 
- Loop Invariant
	- Set of statements that remains true each time the loop body is executed
- Some programmers address the symptom of the  problem by adding a software patch
- off-by-one - Most common error associated with loops
- Loops are harder to debug than sequence and selection structures