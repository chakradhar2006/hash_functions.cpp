# Hash Functions & Data Structures in C++ (`hash_functions.cpp`)

This repository contains modular C++ implementations of common data structure and algorithmic problems, focusing heavily on **Hash Tables**, collision resolution techniques, and practical systems management.

---



### 1. Product Inventory System (`Product Inventory System`)
* **File:** `Product Inventory System` ([View Code](https://github.com/chakradhar2006/hash_functions.cpp))
* **Description:** A console-based inventory management application utilizing a fixed-size hash table and **linear probing** to handle hash collisions. 
* **Data Structure (`struct Product`):**
  * `int code`: Unique product identifier (used as the hash key).
  * `int stock`: Available quantity of the product.
  * `float price`: Unit price of the product.
* **Core Logic & Algorithm:**
  * **Hash Function:** Uses the modulo operator (`index = code % tableSize`) to map product codes to table indices.
  * **Collision Resolution:** Implements linear probing (`index = (index + 1) % tableSize`) to find the next available slot when a collision occurs.
  * **Initialization:** Sets all empty table slots to `-1` to distinguish them from valid product entries.
  * **Operations:** Supports dynamic product insertion, traversal/inventory display, and key-based searching with O(1) average time complexity.

### 2. Library Management System (`library Management`)
* **Description:** *(Add brief overview for your library management implementation)*
* **Key Features:** Book record tracking, issue/return logging, and search utilities.

### 3. Parking System (`parking_system`)
* **Description:** *(Add brief overview for your parking management implementation)*
* **Key Features:** Slot allocation, vehicle tracking, and availability status updates.

---


### Prerequisites
* A C++ compiler supporting C++11 or later (e.g., `g++`, `clang++`, or MSVC).

### Compilation & Execution
To compile and run any of the modules, use your terminal:

```bash
# Example for compiling the Product Inventory System
g++ -o inventory "Product Inventory System"
./inventory
