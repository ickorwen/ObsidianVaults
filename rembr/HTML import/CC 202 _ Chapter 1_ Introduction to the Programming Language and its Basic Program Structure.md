 

 

CC 202 | Chapter 1: Introduction to the Programming Language and its Basic Program Structure

Made with

# CC 202 | Chapter 1: Introduction to the Programming Language and its Basic Program Structure

Early Calculation Devices:

Abacus

calculation tool that uses sliding counters

Leibniz device

“Stepped Reckoner”

mechanical calculator by Gottfried Wilhelm Leibniz

stepped drum mechanism

Jacquard’s Loom

mechanical loom, uses punch cards

Early Computer-like Machines: (MEUV)

Mark I

first large-scale automatic digital computers

50ft long

ENIAC

UNIVAC

1st commercial digital computer in U.S.

Von-Neumann Architecture

a system where a computer’s memory stores data & program instructions

4 Key Components:

CPU - calculates & executes instructions

Memory - stores data & instructions

I/O Devices - allow communication

CU - directs operations of CPU & memory

Categories of Computers:

Mainframe computers

Midsize computers

Micro computers(PCs)

Elements of a Computer System:

CPU

Hardware

Software

Main Memory

Secondary Storage

I/O Devices

CPU

brain of computer, carries logical & arithmetic operations

most expensive

RAM

direct connection to CPU

programs/data must be loaded into main memory before executed/manipulated

volatile nature of RAM

Main Memory

an ordered sequence of memory cells

address - each cell has unique location in main memory, storing instruction/data

Secondary Storage

stores information permanently

Ex.: Hard disks, flash drives, floppy disks, zip disks, CD-ROMs, tapes

Input Devices

feed data and programs into computers

Ex.: Keyboard, mouse , secondary storage

Output Devices

display results

Ex.: Monitor, Printer, secondary storage

Software

programs that do specific tasks

System Programs

control the computer

Operating System

monitors the overall activity of the computer

provides services:

Memory Management

Storage Management

I/O Activities

Application Programs

perform a specific task

Ex.: Word Processors, Spreadsheet, Games

The Language of a Computer

Analog Signals: continuous waveforms used to represent sound

Digital Signals: sequences of 1s and 0s (0 = Low Voltage, 1= High Voltage)

Machine Language: language of a computer; sequences of 0s and 1s

Binary Digit(bit): the digit 0/1

Binary Code(binary number): a sequence of 0s and 1s

Byte: a sequences of 8 bits

Kilobyte(KB): 212^121﻿0^00﻿ bytes = 1024 bytes

ASCII(American Standard Code for Information Interchange): has 128 characters

EBCDIC(Extended Binary Coded Decimal Interchange Code)

used by IBM, 256 characters

Bits - building blocks of digital communication and data storage

Binary Numbers - are used to represent everything in a computer

(Binary code 1010 might represent different things depending on its context)

B, K, M, G, T, P, E, Z (*, Kilo, Mega, Giga, Tera, Peta, Exa, Zetta)

Unicode

65536 characters

2 bytes are needed to store a character

Evolution of Programming Languages

early computers were programmed into machine language

Assembly language instructions are mnemonic

Assembler

translates a program written in assembly language into machine language

wages = rate * hours; = LOAD rate, MULT hour, STOR wages

Examples of High-level languages:

Basic, FORTRAN, COBOL, Pascal, C, C++, C#, Java

Compiler

translates program written in high-level language into machine language

Processing a C++ Program

To Execute a C++ Program:

use an editor to create a source program in C++

preprocessor directives begin with #, and are processed by the preprocessor

use the compiler to:

check if program obeys language rules

translate into machine language(object program)

Linker - combines object program /w other programs provided by SDK to create executable code

Library - contains prewritten code you can use

Loader - loads executable program into main memory

Execute the program

Some IDEs do everything /w Build or Rebuild command

Analysis-Coding-Execution Cycle

Algorithm - step-by-step problem solving process, solution achieved in finite amount of time

programming is a process of problem solving

Step 1: Analyze the Problem

outline the problem & its requirements

design steps or an algorithm to solve the problem

Step 2: Implement the Algorithm

implement the algorithm in code

verify that the algorithm works

Step 3: Maintenance

use and modify the program if the problem domain changes

thoroughly understand problem & all requirements (user interaction, manipulate data, output?)

if the problem is complex, divide into subproblems

think of the problem as a “step-by-step” process

check the correctness of algorithm

write equivalent code in high-level language

enter the program using text editor

different programming language, different syntax & semantics

run code through compiler

if compiler generates errors, look at code and remove errors, run it again

if no syntax errors, compiler generates equivalent machine code

linker links machine code /w system resources

after it’s compiled & linked, loader can place program into main memory for function

execute

compiler guarantees that the program follows the rules of the language

does not guarantee that the program will run correctly

Logical Error - program ran smoothly but /w unexpected results

Programming Methodologies

2 Popular Approaches to Programming Design:

Structured Design

dividing a problem into smaller subproblems

Structured Programming - implemented a structured design

Structured Design a.k.a.:

Top-down/Bottom-up design

Stepwise refinement

Modular programming

Object-Oriented Design

identify components called objects

determine how objects interact /w each other

specify relevant data and possible operations to be performed on that data

each object consists of data and operations on that data

an object combines data & operations on the data into a single unit

OOP(Object-Oriented Programming) Language: a programming language that implements OOD

must learn how to represent data in computer memory, how to manipulate data, and how to implement operations

write algorithms and implement them in a programming language

use functions to implement algorithms

learn how to combine data and operations on the data into a single united(object)

OOD is used with structured design

C++

was designed to implement OOD

evolved from C

designed by Bjarne Stroustrup at Bell Labs(1980s)

many different C compilers were available

C++ programs were not always portable from one compiler to another

mid-1998, ANSI/ISO C++ Language standards were approved