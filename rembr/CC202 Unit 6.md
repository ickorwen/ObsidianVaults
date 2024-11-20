### User Defined Functions
- often called **modules**
- miniature programs that can be combined to form larger programs

### Predefined Functions
- organized into separate libraries
	- I/O functions are in iostream header
	- Math functions are in cmath header
- must include the header file using an include statement

### User Defined Functions

- Value-returning functions
	- have a return type
	- uses return statement
- Void functions
	- do not have a return type
	- no return statement

#### Value-returning Functions
- Include the appropriate header file in your program using the include statement
- function header(aka heading)
	- Return type - Specifies the type of value the function will return; Functiontype, data type; return type
	- Function Name - The identifier for the function, such as abs in this case. This name is used to call the function in the program.
	- Parameter list - Enclosed in parentheses after the function name, this lists the input values the function expects.
	- Opening Brace - marks beginning of function body (certain langs only)
	- together with body forms the definition of function

- Formal Parameter - variable declared in the heading
- Actual parameter - variable or expression listed in a call to a function

- return statement - passes value outside function
- Function Prototype - 
	- function heading without the body of the function
	- Not necessary to specify the variable name
	- Data type of each parameter must be specified

### Flow of Execution
- Execution always begins at the first statement in the function main
- Function prototypes appear before any function definition


### Void Functions
- no return type

- Value parameter - a formal parameter that receives a copy of the content of corresponding actual parameter
	- The value of the corresponding actual parameter is copied into it
- Reference parameter - a formal parameter that receives the location (memory address) of the corresponding actual parameter

### Scope of an identifier: 
- Defines where an identifier can be accessed in the code, including **local** and **global identifiers**.
	- **local** - declared within a function
	- **global** - declared outside of every function definition
- C++ does not support nested functions, meaning one function cannot be defined within another.
- The **scope resolution operator** (`::`) can be used to access global variables that may have the same name as local identifiers.
- Rules when an identifier is accessed:
	- Global identifiers are accessible by a function or block if:  
		- Declared before function definition  
		- Function name different from identifier  
		- Parameters to the function have different names  
		- All local identifiers have different names
	- Nested block
		- Identifier accessible from declaration to end of block in which it is declared  
		- Within nested blocks if no identifier with same name exists 
			- Scope of function name similar to scope of identifier declared outside any block

### Static and Automatic Variables
- **Automatic variables** are created upon entering a block and destroyed upon exiting.
- **Static variables** maintain their value throughout the execution of the program, allowing for persistent state.

### Debugging
- **Driver programs** are used to test specific functions, ensuring that they perform as expected.
- **Function stubs** serve as placeholders for functions that are not fully implemented, allowing for incremental testing.

### Function Overloading
- C++ allows multiple functions to share the same name as long as their **parameter lists** differ; 
- **Function signature:** 
	- the name and formal parameter list of the function
	- does not include return type
- Two functions are said to have different formal parameter lists if both functions have either:
	- A different number of formal parameters
	- If the number of formal parameters is the same, but the data type of the formal parameters differs in at least one position
- Overloaded functions must have different function signatures