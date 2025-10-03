# 💻 C++ EXPERIMENTS

A curated collection of C++ programs for practice and learning, designed with simplicity and clarity in mind.

---

## 👨‍🎓 Student Information

- **Name:** Updesh Arora  
- **PRN:** 24070123124  
- **Branch:** ENTC  
- **Class:** B-3

---
# EXP-18_Stack.cpp

## AIM
To implement a **stack data structure** using C++ classes and perform **Push** and **Pop** operations while handling **overflow** and **underflow** conditions.

## TOOLS REQUIRED
- C++ Compiler (e.g., g++, clang++)
- Text Editor / IDE (VS Code, Code::Blocks, etc.)
- Terminal/Command Prompt to compile and run the program

## THEORY
A **stack** is a **linear data structure** that follows the **Last-In-First-Out (LIFO)** principle. The last element inserted into the stack is the first one to be removed.  

### Key Operations
1. **Push** – Insert an element at the **top** of the stack.  
   - Before pushing, check if the stack is **full** to avoid overflow.  
2. **Pop** – Remove the element from the **top** of the stack.  
   - Before popping, check if the stack is **empty** to avoid underflow.  
3. **Top/Peek** – Retrieve the element at the top without removing it.  
4. **isEmpty** – Check if the stack has no elements.  
5. **isFull** – Check if the stack has reached its maximum capacity (for array-based stacks).

### Implementation Notes
- Stacks can be implemented using **arrays** or **linked lists**.  
- Using a **class in C++** allows encapsulation of stack data and operations.  
- Proper error handling for **overflow** and **underflow** ensures the program runs safely.

### Advantages of Stack
- Simple and efficient for certain problems like **expression evaluation**, **undo operations**, and **function call management**.  
- Provides controlled access to data, making it **safe and predictable**.

### Practical Applications
- **Expression conversion** (infix to postfix/prefix) and evaluation.  
- **Backtracking algorithms** (e.g., maze solving, DFS in graphs).  
- **Undo/Redo** in text editors.  
- **Function call stack** in program execution.

## EXPERIMENT 19(A): STACK IMPLEMENTATION USING CLASS IN C++

### ALGORITHM
1. **START**  
2. Define a class `Stack` with:  
   - Data members: `arr` (array pointer), `top` (index of top element), `capacity` (size of stack).  
   - Constructor to initialize `arr`, `top = -1`, and `capacity`.  
   - Member functions:  
     - `isFull()` → returns true if `top == capacity-1`.  
     - `isEmpty()` → returns true if `top == -1`.  
     - `push(int x)` → add element `x` to stack if not full; else display overflow.  
     - `pop()` → remove and return top element if not empty; else display underflow.  
     - `peek()` → return top element without removing it.  
   - Destructor to free allocated memory.  

3. In `main()`:  
   - Create a `Stack` object with a specific size.  
   - Use `push()` to add elements to the stack.  
   - Use `peek()` to display the top element.  
   - Use `pop()` to remove elements from the stack.  
   - Handle cases where stack is **overflowed** or **underflowed**.  

4. **STOP**

## CONCLUSION

In this experiment, we successfully implemented a **stack** using a class in C++ and demonstrated the basic stack operations: **push**, **pop**, and **peek**.  
We learned how to manage the **top pointer** to track the current element and handle boundary conditions like **stack overflow** and **underflow**.  

This exercise reinforced the concept of **LIFO (Last-In-First-Out)** behavior in stacks and how object-oriented programming facilitates encapsulation and modular design for data structures.
