# Pointer Basics and Operations in C++ 

## Aim

To study and implement **C++ Pointer basics** and perform various operations using pointers, including:

* Pointer declaration and basic usage
* Pointer arithmetic
* Finding the difference between two pointers
* Traversing arrays with pointers
* Printing strings using pointers
* Reversing arrays and strings using pointers

---

## Tools Used

* VS Code
* Any online compiler such as Programiz, Replit, or OnlineGDB

---

## Theory

A **pointer** in C++ is a variable that stores the memory address of another variable.
Pointers are essential for working with **dynamic memory allocation**, **arrays**, **strings**, and **low-level memory manipulation**.

**Important facts about pointers:**

* Pointers must be of the **same type** as the variable they point to.
* The `&` operator gets the **address** of a variable.
* The `*` operator **dereferences** a pointer to get the value at its address.
* Pointer arithmetic allows moving between elements in arrays:

  * `p++` moves to the **next element** of the pointer’s type.
  * `p--` moves to the **previous element**.
  * `p + n` moves forward by `n` elements.
* For `char*` pointers, printing directly will output the string unless explicitly cast to `(void*)`.
* Strings in C++ are stored as arrays of characters, ending with a \0 null terminator.

---

## Algorithms

### 1) Pointer Basics – Printing Address and Values

**Goal:** Demonstrate pointer declaration, initialization, and dereferencing.
**Steps:**

1. Start the program.
2. Declare variables of different types (`int`, `float`, `double`, `char`, `bool`).
3. For each variable:

   * Declare a pointer of the same type.
   * Assign it the variable’s address using `&`.
   * Print the variable’s value.
   * Print the variable’s address using the pointer.
   * Print the pointer’s own value (which is the address).
   * Print the dereferenced pointer to show the value stored at that address.
4. Stop the program.

---

### 2) Basic Pointer Arithmetic

**Goal:** Show how incrementing a pointer changes its stored address based on the data type size.
**Steps:**

1. Start the program.
2. Declare variables of different types.
3. For each variable:

   * Create a pointer pointing to it.
   * Print the original address stored in the pointer.
   * Print the size of the variable’s type using `sizeof()`.
   * Increment the pointer using `p++`.
   * Print the new address after increment.
4. Observe that the difference in addresses equals the size of the data type.
5. Stop the program.

---

### 3) Difference Between Two Pointers

**Goal:** Calculate the difference between values or positions of two pointers.
**Steps:**

1. Start the program.
2. Declare and initialize an integer array with fixed values.
3. Assign two pointers to different positions in the array.
4. For **value difference**:

   * Dereference both pointers.
   * Subtract one value from the other.
5. For **address difference**:

   * Directly subtract one pointer from the other.
   * The result gives the number of elements between them.
6. Print the result.
7. Stop the program.

---

### 4) Traversing an Array Using Pointers

**Goal:** Access all array elements using pointer increment.
**Steps:**

1. Start the program.
2. Declare and initialize an array.
3. Create a pointer pointing to the first element of the array.
4. Loop from `0` to `n-1` (array size - 1):

   * Print the current address stored in the pointer.
   * Print the value stored at that address (dereferenced pointer).
   * Increment the pointer to move to the next element.
5. Stop the program.

---

### 5) Printing a String Using Pointers

**Goal:** Display each character of a string using pointer traversal.
**Steps:**

1. Start the program.
2. Declare and initialize a character array (string).
3. Create a pointer pointing to the first character.
4. While the character pointed to is not the null terminator`:

   * Print the character.
   * Increment the pointer to move to the next character.
5. Stop the program.

---

### 6) Reversing an Array Using Pointers

**Goal:** Display array elements in reverse order using pointer decrement.
**Steps:**

1. Start the program.
2. Declare and initialize an array.
3. Create a pointer pointing to the **last element** of the array (`arr + n - 1`).
4. Loop from `n-1` to `0`:

   * Print the current value pointed to by the pointer.
   * Decrement the pointer to move to the previous element.
5. Stop the program.

---

### 7) Reversing a String Using Pointers

**Goal:** Print a string in reverse order using pointer traversal.
**Steps:**

1. Start the program.
2. Declare and initialize a string (character array).
3. Use `strlen()` to find the length of the string.
4. Create a pointer pointing to the last character (`str + length - 1`).
5. Loop backwards from `length - 1` to `0`:

   * Print the character pointed to by the pointer.
   * Decrement the pointer to move one position back.
6. Stop the program.

---

## Outcome

By completing these programs, you will be able to:

* Declare, initialize, and use pointers with various data types.
* Apply pointer arithmetic to navigate memory.
* Compare pointers to find differences in values and positions.
* Traverse arrays and strings using only pointers.
* Reverse arrays and strings using pointer operations.
* Strengthen understanding of memory addresses, data type sizes, and pointer manipulation in C++.

---
