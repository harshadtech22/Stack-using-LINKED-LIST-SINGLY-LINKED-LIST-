# 📚 Stack Implementation using Singly Linked List in C

## 📌 Project Overview

This project demonstrates the implementation of a **Stack Data Structure (LIFO - Last In First Out)** using a **Singly Linked List (SLL)** in the C programming language.

Unlike array-based stacks, this implementation uses dynamic memory allocation, allowing the stack to grow and shrink efficiently at runtime.

---

## 🚀 Features

* **Push Operation** → Insert an element into the stack
* **Pop Operation** → Remove the top element from the stack
* **Peek Operation** → View the top element without removing it
* **Display Operation** → Print all stack elements (top to bottom)
* Handles:

  * Stack Overflow (memory allocation failure)
  * Stack Underflow (empty stack)

---

## 🧠 Data Structure Concept

* Each node in the linked list represents a stack element
* A pointer called **TOS (Top Of Stack)** keeps track of the top node
* Operations are performed at the **beginning of the linked list**

---

## ⚙️ How It Works

* **Push**

  * Create a new node using `malloc()`
  * Insert it at the beginning
  * Update TOS pointer

* **Pop**

  * Remove the first node
  * Return its value
  * Free memory using `free()`

* **Peek**

  * Return the value of the top node without deletion

* **Display**

  * Traverse the linked list from top to bottom

---

## 📂 Project Structure

```bash
stack_sll.c
README.md
```

---

## 🖥️ Sample Menu

```bash
1. Push
2. Pop
3. Display All
4. Display Peek Value
```

---

## ▶️ How to Compile and Run

### Step 1: Compile

```bash
gcc stack_sll.c -o stack_sll
```

### Step 2: Run

```bash
./stack_sll
```

---

## 💻 Example Execution

```bash
Enter the option: 1
Enter a number to be pushed: 10

Enter the option: 1
Enter a number to be pushed: 20

Enter the option: 3
The Stack Elements are:
20
10

Enter the option: 2
Popped Element is 20

Enter the option: 4
Peek Element is 10
```

---

## ⚠️ Error Handling

* **Stack Underflow**

  * Occurs when attempting to pop or peek from an empty stack

* **Stack Overflow**

  * Occurs if `malloc()` fails (rare but handled)

---

## 🛠️ Requirements

* GCC Compiler
* Basic knowledge of:

  * Pointers
  * Dynamic Memory Allocation
  * Linked Lists

---

## 📌 Important Notes

* `malloc()` is used for dynamic memory allocation
* `free()` ensures no memory leaks after pop operations
* Avoid using `fflush(stdin)` in modern C as it leads to undefined behavior

---

## 🔮 Future Improvements

* Add size tracking of stack
* Implement stack using doubly linked list
* Add file-based input/output
* Convert into modular code with header files

---

## 📚 References

* GeeksforGeeks – Stack Data Structure
* GeeksforGeeks – Stack using Linked List
* TutorialsPoint – Stack in Data Structures

---

## 👨‍💻 Author

Developed as part of Data Structures learning using C.

---

## 📜 License

This project is open-source and free to use for educational purposes.

---

## ⭐ Contribution

Feel free to fork this repository and enhance the implementation with additional features or optimizations.
