
---

## **Unit 3: Inheritance and Composition**

### **Objectives**

In this chapter, you will:

- Learn about **inheritance**.
- Learn about **derived** and **base classes**.
- Redefine the **member functions** of a base class.
- Examine how the **constructors** of base and derived classes work.
- Learn how to construct the **header file** of a derived class.
- Learn about the **C++ stream hierarchy**.
- Explore three types of **inheritance**: **public, protected, private**.
- Learn about **composition (aggregation)**.
- Become familiar with the **three basic principles of object-oriented design**.

---

## **1. Introduction**

Two common ways to relate two classes in a meaningful way are:

1. **Inheritance** (**"is-a" relationship**)
2. **Composition (aggregation)** (**"has-a" relationship**)

---

## **2. Inheritance**

- **Definition**: **Inheritance** represents an **"is-a" relationship** in object-oriented programming.
- **Example**: "Every **employee** is a **person**."
- **Purpose**: Allows the creation of **new classes** from **existing classes**.
- **Base Class**: The **original class**.
- **Derived Class**: The **new class** created from a **base class**.
- A **derived class** inherits the **properties** of its **base class**.
- Helps **reduce software complexity**.

### **Types of Inheritance**

1. **Single Inheritance** – The **derived class** has **one base class**.
2. **Multiple Inheritance** – The **derived class** has **more than one base class**.
3. **Public Inheritance** – All **public members** of the **base class** are inherited as **public** in the **derived class**.

### **Syntax of a Derived Class**

```cpp
class DerivedClass : memberAccessSpecifier BaseClass {
   // Member list
};
```

- **memberAccessSpecifier** can be **public, protected, or private** (**default**).
- **Private members** of a **base class** are **not directly accessible** in the **derived class**.

### **Access Modifiers in Inheritance**

|**Inheritance Type**|**Public Members of Base**|**Protected Members of Base**|**Private Members of Base**|
|---|---|---|---|
|**Public**|Public in derived class|Protected in derived class|**Not accessible**|
|**Protected**|Protected in derived class|Protected in derived class|**Not accessible**|
|**Private**|Private in derived class|Private in derived class|**Not accessible**|

---

## **3. Redefining (Overriding) Member Functions of the Base Class**

- **To redefine a public member function** in the derived class:
    - It must have the **same name, number, and types of parameters**.
    - To call the **base class function**, use:
        
        ```cpp
        BaseClass::functionName();
        ```
        
- **Example**:
    
    ```cpp
    class Base {
    public:
        void show() { cout << "Base class function"; }
    };
    
    class Derived : public Base {
    public:
        void show() { cout << "Derived class function"; }
    };
    ```
    

---

## **4. Constructors & Destructors in Derived Classes**

- **Derived class constructor** **cannot directly access private members** of the **base class**.
- It can **only initialize** public **member variables** of the **base class**.
- **When a derived object is created**:
    - It must **execute a constructor** of the **base class**.
    - **Base class constructor** executes **first**.
- **Destructor Execution**:
    - When a **derived class object** goes **out of scope**, its **destructor is called first**, then the **base class destructor**.

### **Example: Constructor Execution Order**

```cpp
class Base {
public:
    Base() { cout << "Base Constructor\n"; }
    ~Base() { cout << "Base Destructor\n"; }
};

class Derived : public Base {
public:
    Derived() { cout << "Derived Constructor\n"; }
    ~Derived() { cout << "Derived Destructor\n"; }
};

int main() {
    Derived obj;
    return 0;
}
```

**Output:**

```
Base Constructor  
Derived Constructor  
Derived Destructor  
Base Destructor  
```

---

## **5. Composition (Aggregation)**

- Represents a **"has-a" relationship**.
- A class has **member variables** that are **objects of another class**.
- **Example**: A **Car** class contains an **Engine** class.

### **Example: Composition**

```cpp
class Engine {
public:
    Engine() { cout << "Engine created\n"; }
};

class Car {
    Engine engine; // Composition
public:
    Car() { cout << "Car created\n"; }
};
```

---

## **6. C++ Stream Classes**

- **ios**: The **base class** for all **stream classes**.
- **istream and ostream**:
    - **istream** handles **input operations**.
    - **ostream** handles **output operations**.
    - **ifstream/ofstream** are used for **file I/O**.
    - Defined in **fstream** header file.

---

## **7. Object-Oriented Design (OOD) & Object-Oriented Programming (OOP)**

### **Three Basic Principles**

1. **Encapsulation** – Combines **data and operations** into a **single unit**.
2. **Inheritance** – Allows **code reuse** by **creating new objects from existing ones**.
3. **Polymorphism** – Enables **the same function/operator to perform different operations**.

### **Example of Polymorphism**

```cpp
class Base {
public:
    virtual void display() { cout << "Base class"; }
};

class Derived : public Base {
public:
    void display() override { cout << "Derived class"; }
};
```

---

## **8. Identifying Classes, Objects, and Operations**

- **To find classes**:
    - Identify **nouns** in the problem description.
- **To find operations**:
    - Identify **verbs** in the problem description.
- **Example**:  
    **Problem**: "Write a program to input the dimensions of a cylinder and calculate and print the surface area and volume."
    - **Nouns**: Cylinder, dimensions, surface area, volume → **Classes**.
    - **Verbs**: Input, calculate, print → **Operations**.

---

## **9. Summary**

- **Inheritance** and **composition** are ways to **relate classes**.
- **Inheritance** represents an **"is-a"** relation.
- **Single inheritance** has **one base class**, while **multiple inheritance** has **more than one base class**.
- **Composition** represents a **"has-a"** relation.
- **Base class private members** are **not directly accessible** in derived classes.
- A **derived class can override** functions of the **base class**.
- **Encapsulation, inheritance, and polymorphism** are the **three key principles** of **OOP**.

---
