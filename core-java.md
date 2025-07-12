
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

## Static Method - 
- A static method in Java belongs to the class rather than any object and can be called without creating an object. 
- It is declared using the static keyword and can only access static data directly (not instance variables).

## Static Block - 
- A static block in Java is used to initialize static variables and runs once when the class is loaded, before the main() method. 
- It’s executed automatically by the JVM without creating any object.

## this() & super() method -
- this() calls another constructor in the same class and helps avoid code duplication.

- super() calls a constructor from the parent class to reuse or initialize inherited properties.

- Both must be the first statement in a constructor.


## Final keyword - 
- Final keyword we can use with variable, method, and class.

- Final Variable: Value cannot be changed (acts as a constant).

- Final Method: Cannot be overridden by subclasses.

- Final Class: Cannot be inherited (no subclass allowed).


## Difference between Final and Static keywords - 
- final makes variables constant, methods non-overridable, and classes non-inheritable.

- static makes variables and methods belong to the class, not to objects. (can access without any object).


## Wrapper calss - 
- Wrapper class in Java is used to convert primitive data types into objects. Java provides a wrapper class for each primitive type, like int → Integer, char → Character, etc.

- They are useful when:

    - Working with collections like ArrayList (which only store objects),

    - Using utility methods (e.g., Integer.parseInt()),

    - Performing autoboxing (primitive to object) and unboxing (object to primitive) automatically.

## Dynamic Method Dispatch - 
- Dynamic Method Dispatch in Java is the process where the method call is resolved at runtime, not compile time. 
- It occurs when a parent class reference points to a child class object, and the overridden method in the child class gets called. 
- This enables runtime polymorphism, allowing Java to decide which method to execute based on the actual object.
