
# Core java

## LTS - (Long term support)
- it means a version of Java that will receive extended updates and support from Oracle or other vendors for a longer period (typically several years). Ideal for enterprise and production use.

## How java works -
- we write java code then compiler (javac) can convert this code into byte code

- JVM (java virtual machine) can execute only byte code

## Stack and Heap - 
- Stack memory -  stores local variables and function calls; it’s fast and automatically managed.

- Heap memory - stores objects and dynamic data; it's larger, slower, and managed manually or by a garbage collector.

- Stack is short-term memory, while heap is for long-term use during program execution.

## Jagged Array - 
- A jagged array is an array of arrays with different lengths for each row.

- It’s like a 2D array, but each row can have a different number of elements.

## String - 
- How immutable string works - 
    - String Constant Pool - this is a special memory area in Java used to store unique string literals. It helps in saving memory and improving performance by avoiding duplicate string objects.

    - Both Strings s1 and s2 will point to the same object in the String Constant Pool, instead of creating two separate objects.

    - you can check this with comparing this two Strings with (==) operator and .equals() method.

    - (==) check its variables content with memory address and .equals() check only content of variable.

- How mutable string works - 
    - StringBuffer in Java is a mutable, thread-safe class used to modify strings without creating new objects. It supports operations like append, insert, delete, and reverse, and is synchronized for use in multi-threaded environments.


## Static Variables - 
- A static variable in Java is shared among all instances of a class and is stored in memory only once. 
- It belongs to the class, not objects, and is declared using the static keyword. It can be accessed directly using the class name.
