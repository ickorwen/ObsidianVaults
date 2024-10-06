---
tags:
  - West
---

## **Chapter 1: Overview of Computers and Programming Languages**

### Key Points:
- **Without software**, a computer is useless.
- Software is developed using **programming languages**.
- **C++** is a widely-used programming language suitable for various tasks.

### History of Computers:
- Early Calculation Devices:
	1. Abacus
		- calculation tool that uses sliding counters
	2. Leibniz device
		- “Stepped Reckoner”
		- mechanical calculator by Gottfried Wilhelm Leibniz
		- stepped drum mechanism
	3. Jacquard’s Loom
		- mechanical loom, uses punch cards
- **Early computers**: 
	1. **Mark I**
		- first large-scale automatic digital computers
		- 50ft long
	2. ENIAC (Electronic Numerical Integrator and Computer)
	3. UNIVAC (Universal Automatic Computer)
	4. ==**Von-Neumann Architecture**==: 
		- a system where a computer’s memory stores data & program instructions
		- 4 Key Components:
			- ==CPU==: Executes instructions.
			- ==Memory==: Stores data.
			- ==Input/Output== Devices: Communication interface.
			- ==Control== Unit: Directs CPU operations.

- **Categories of Computers**: 
	- Mainframes, 
	- Mid-size, 
	- Micro (PCs).

### Computer System Components:

**Hardware**: 
- **CPU**: 
	- The brain of the computer; performs calculations.
- **RAM (Main memory)**:
	- Directly connected to the CPU.
	- Volatile – data is lost when powered off.
	- Programs and data must be loaded into RAM for processing.
- **Secondary Storage:**
	- stores information permanently
	- Ex.: Hard disks, flash drives, floppy disks, zip disks, CD-ROMs, tapes
- **Input Devices:** 
	- feed data and programs into computers
	- Keyboard, Mouse, Storage.
- **Output Devices:** 
	- display results
	- Monitor, Printer, Storage.
**Software**:
- Programs that do specific tasks
- **System programs** - Control the computer.
	- Operating System
		- monitors the overall activity of the computer
		- provides services:
			- Memory Management
			- Storage Management
			- I/O Activities
- **Application programs** (e.g., Word processors, Spreadsheets) perform specific tasks.

### The Language of a Computer:


**Analog Signals:** continuous waveforms used to represent sound

**Digital Signals:** sequences of 1s and 0s (0 = Low Voltage, 1= High Voltage)


Machine Language: language of a computer; sequences of 0s and 1s

**Assembly language**: Mnemonics with an assembler to translate into machine code.

**High-level languages**: C++, Java, Python, etc. Use a compiler to translate to machine code.


**Binary Digit(bit):** the digit 0/1, building blocks of digital communication and data storage
**Bytes**: 8 bits
**Binary Code(binary number):** a sequence of 0s and 1s

**ASCII(American Standard Code for Information Interchange):** has 128 characters
 - 128 characters

**EBCDIC(Extended Binary Coded Decimal Interchange Code)**
 - used by IBM, 256 characters

**Compiler**
 - translates program written in high-level language into machine language
 
### Example in C++:
```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "My first C++ program." << endl;
    return 0;
}
```
- Compiled and linked to produce an executable program.

### To Execute a C++ Program:

1. use an editor to create a source program in C++
2. **preprocessor directives** begin with #, and are processed by the preprocessor
3. use the **compiler** to:
    - check if program obeys language rules
    - translate into machine language(**object program**)
4. **Linker** - combines object program /w other programs provided by SDK to create executable code
    - **Library** - contains prewritten code you can use
5. **Loader** - loads executable program into main memory
6. Execute the program
	- Some IDEs do everything /w Build or Rebuild command

### Problem Analysis–Coding–Execution Cycle:
1. **Analyze** the problem.
2. **Implement** the solution in code.
3. **Maintenance**: Modify if necessary.

### Programming Methodologies:
- **Structured programming**: Break problems into subproblems (Top-down, Modular).
- **Object-Oriented Programming (OOP)**: Combines data and functions into objects.

### ANSI/ISO Standard C++:
- Standardized in **1998** for portability across compilers.

### Summary:
- **Computer system**: Hardware (CPU, memory), Software (system & application).
- **Algorithm**: Step-by-step problem-solving process.
- **Programming**: Analyze, code, and maintain.

---
## **Chapter 2: Basic Elements of C++**

### **Objectives:**

- Understand functions, special symbols, and identifiers.
- Learn simple data types, arithmetic expressions, and assignment statements.
- Explore string data types and input/output statements.
- Use increment/decrement operators, preprocessor directives, and debugging.

### **C++ Program Structure:**

- **Program**: A collection of functions; `main()` is mandatory.
- **Comments**: Use `//` for single-line comments and `/* */` for multi-line.
- **Output Statement**: `cout <<` displays data; `endl` moves to a new line.

### **Tokens in C++:**

- **Special Symbols**: `+`, `-`, `*`, `/`, `<=`, etc.
- **Reserved Words**: `int`, `float`, `double`, `void`, etc. (cannot be redefined).
- **Identifiers**: Names for variables, functions, etc. (case-sensitive).

### **Data Types:**

- **Simple Data Types**:
    - **Integral**: `char`, `int`, `long`, `bool`.
    - **Floating-point**: `float`, `double`.
    - **Enumeration**: User-defined types.
- **Variable Declaration**: E.g., `int counter;`, `double rate;`.

### **Arithmetic Operators & Expressions:**

- Operators: `+`, `-`, `*`, `/`, `%`.
- Precedence: `*`, `/`, `%` before `+`, `-`.
- **Mixed Expressions**: C++ converts integers to floating-point if mixed.

### **Type Conversion (Casting):**

- **Implicit**: Automatic type conversion.
- **Explicit**: Use `static_cast<dataType>(expression)`.

### **String Type:**

- **String**: Sequence of characters enclosed in double quotes (e.g., `"Hello"`).
- **Length**: Position of the first character is `0`.

### **Input Statements:**

- Use `cin >>` for input (e.g., `cin >> miles;`).
- Multiple inputs: `cin >> feet >> inches;`.

### **Increment/Decrement Operators:**

- Pre-increment (`++var`), post-increment (`var++`), pre-decrement (`--var`), post-decrement (`var--`).

### **Preprocessor Directives:**

- Use `#include` to include libraries like `<iostream>`.
- Preprocessing happens before compilation.

### **Program Structure:**

- **Main Function**: Starts with `int main()`.
- **Declaration Statements**: Define variables, constants.
- **Executable Statements**: Perform actions like calculations, input/output.

### **Debugging Syntax Errors:**

- Compiler highlights errors like missing semicolons or undeclared variables.

---
## **Chapter 3: Input/Output**

### Key Concepts:

- **Stream**: A sequence of bytes (characters) from a source to a destination.
    - **Input Stream**: Data flows from an input device to the computer.
    - **Output Stream**: Data flows from the computer to an output device.

### I/O Streams in C++:

- Use the **iostream** header to handle input/output operations.
- **cin**: Standard input (keyboard).
- **cout**: Standard output (screen).

### Input Operations:

- **Extraction Operator (>>)**:
    - Used to read data (e.g., `cin >> variable;`).
    - Skips whitespaces and distinguishes between characters and numbers.
    - Input failure occurs when the wrong type of data is entered.

### Common I/O Functions:

- **get()**: Reads a single character (including whitespace).
- **ignore()**: Skips characters in input.
- **putback()**: Puts back the last character read by get().
- **peek()**: Returns the next character without extracting it.

### Output Formatting:

- Use **manipulators** to format output:
    - **endl**: Inserts a new line.
    - **setprecision**: Sets the number of decimal places.
    - **setw**: Specifies the number of output columns.
    - **fixed**: Displays numbers in fixed-point notation.
    - **showpoint**: Forces the display of the decimal point and trailing zeros.

### File Input/Output:

1. Include the **fstream** header.
2. Declare file stream variables.
3. Open files using input/output functions (e.g., `ifstream` for input, `ofstream` for output).
4. Close the files when done.

### Handling Errors:

- **Input failure**: Occurs when reading invalid data. Use the **clear()** function to reset the input stream.
- **Debugging**: Use `cout` statements to identify and fix logic errors.
---
## **Chapter 4: Control Structures I (Selection)**

### Key Concepts:

- **Control Structures**:
    - **Sequence**: Executes statements in order.
    - **Selection (Branching)**: Makes decisions (if, if...else, switch).
    - **Repetition**: Loops.
    - **Function Calls**: Executes functions.

### Relational Operators:

- Used for comparisons.
- **Examples**:
    - `8 < 15`: true.
    - `6 != 6`: false.
    - Can be applied to characters and strings.

### Logical (Boolean) Operators:

- Combine logical expressions.
- **Operators**:
    - `&&` (AND), `||` (OR), `!` (NOT).

### Selection Structures:

- **if** and **if...else**:
    
    - One-way or two-way selection.
    - Use with Boolean expressions.
- **Nested if**: Place one `if` within another.
    
- **switch**:
    
    - Handles multi-way selection.
    - Evaluates an expression and executes the matching case.
    - Break statement required after each case to avoid fall-through.

### Short-Circuit Evaluation:

- Logical expressions stop evaluating as soon as the result is known.
    - Example: `(age >= 21) || (x == 5)`.

### Conditional (Ternary) Operator:

- **Syntax**: `condition ? expression1 : expression2`.
    - Example: `max = (a >= b) ? a : b;`.

### Common Pitfalls:

- **Equality (\=\=) vs Assignment (=)**:
    - Mistakenly using `=` instead of `==` can lead to logical errors.

### assert Function:

- Used to terminate a program if a condition is not met.
- **Syntax**: `assert(expression);`.
    - If `expression` is false, the program stops.

### Summary:

- **Control structures**: Sequence, selection (if, switch), repetition.
- **Relational operators**: `==, !=, >, <`.
- **Logical operators**: `&&, ||, !`.
- **Selection**: if, if...else, switch.
- **assert**: Halts execution when a condition is false.
--- 

