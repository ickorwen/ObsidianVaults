CLASSES
OBJECT ORIENTED DESIGN -problem solving methodology
Objects - components of a solution
Class  - a collection of a fixed number f components
member - a component of a class
	- defines a datatype , no memory is allocated
	- dont forget the semicolon after the cloing brace
	- class member can be a variable or a funtion
	- if a member of a class is a variable
		- it is declared like any other variable
		- you cannot initialize a variable whne you declare it
member access specifiers:
private (defautl)
	member cannot be accessed outside class
public 
	member is accesible outside class
protected 

Unified modeling Language (UML) Class Diagrams

UML Notation - used to graphically describe a class and its members
	+ member is public
	- member is private
	# member is protected

Built in operations in cpp classes
	do not apply to classes:
		arithmetic operators
		relational operators
	valid for classes
		member acces
		assignment

Class Scope
	automatic
		created when declaration reached, destroyed when code block exited
	static
		created when declaration reached, destroyed when program is terminated

