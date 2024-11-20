#incomplete

### Types of algorithms

1. Sorting Algorithm
	- used to sort collections of data
	- bubble sort, quick sort, merge sort heap sort and others
					- ![[Pasted image 20241105232302.png]]
2. Search Algorithm
	- used to find a specific piece of information within a collection of data
	- linear search, binary search, jump search, exponential search, Fibonacci search
3. Encryption Algorithm
	- used to encrypt data to protect it from unauthoried access. 
	- AES, RSA, and DES
4. Machine Learning Algorithms
	- have gained an importance and may change the way we analyze data
	- Neural networks
		- machine learning algo modeled on our brains and designed to make decisions. 
		- recommendations algorithms; popular and used by big companies to predict

![[Pasted image 20241105223944.png]]

### Object-Oriented Programming (OOP)
- programming model centered around classes and objects
	- ==class== - properties and behaviours of entities relevant to the program
- allows you to organize your code in a modular and reusable way
- objects have attributes(data) and methods(functions)
- Advantages over simpler paradigms such as procedural programming:
	- ==Simplicity==
		- define variables the closely resemble the properties and behaviors of the real world.
	- ==Modularity==
		- OOP allows you to break your code into small, reusable modules(objects)
	- ==Encapsulation==
		- OOP allows you to hide the internal details of an object and expose only the necessary methods and attributes
	- Inheritance
		- OOP allows you to create classes based on existing classes (parent classes)
			![[Pasted image 20241105225224.png]]
			
### Objects
- ==Object==
	- instance of a class, consists of one/more properties that are key-value pairs defining the characteristics of the object, and methods, whic are functions that define the behaviour of the object.
	- core feature of most programming languages used today. Including ==Javascript, Python, and Java==
	
	```js
		let recipe = {
			recipeName: " Lemon Orange Cake",
			recipeSource: "Taste of Home",
			recipeDetails: function(){
			return recipeName + "from" + recipeSource;
			}
		} 
	```
	- we can access the properties of an object  using bracket notation
	```js
		console.log(recipe.recipeName)
	```


### Popular OOP Languages
#### Java
- first oop that gained commercial popularity
- mobile apps, web apps, enterprise systems

#### Python
- versatile general purpose OOP Language
- data analysis, machine learning, and web development
- known for simplicity, readability, versatility

#### C++
- known for efficiency and hardware interaction capabilities
- high-performance apps like OS, Game engine, embedded systems
- steep learning curve

#### C# 
- modern OOP language that supports  emerging design practices.
- Mobile apps, web apps, cloud based services, games
- simplicity, type safety, extensive libraries

#### Ruby
- flexible,dynamic OOP language
- web apps, scripting, automation
- readbility, expressiveness
	- ==Ruby on Rails Framework==
		- introduced the concept of ==Model-View-Controller== to develop web apps
			- basis for almost all web applications

#### Swift 
- modern, fast OOP language that is used for building iOS, macOS, and watchOS apps
- safety, speed, easy to use

#### JavaScript
- did not start as an OOP language
- acquired OOP characteristics
- can be used for both OOP and procedural programming styles


### Variables
- named storage location in a computer's memory that holds a value
-  ```  =  ```  assignment operator

### Functions / Methods
- block of code the performs a specific task
- defined with a name, can be called or invoked repeatedly from other parts of a program
- provide a way to modularize code
- improve program correctness
- Inputs are called ==Parameters/arguments==
- used extensively in frontend and backend development
- Js has console.log() to print results to the console


### Algorithms
- a set of instructions used to solve a problem.
- most efficient methods for computing tasks
- ==flowchart== or ==pseudocode==
- 