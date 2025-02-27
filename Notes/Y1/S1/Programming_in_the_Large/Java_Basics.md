# Java Basics 
## Overview
Java is `general-purpose` programming language
- compiled
- statically Typed
- OOP
- Memory Safe

Interpreted, read by line and executed
Compiled, first compiled to bytecode then executed

ByteCode allows for machine independence and to run on the JVM

## Types in Lang
Python is `dynamically typed`. the appropriate type used is determined when the program is executed
Java is `statically typed`. Types are checked for scenarios in the compiler

Java needs `;` at the end of a statement
Java needs a `main` method to enter the process

```Java 
public static void main(String[] args) {
    int nums1=10;
    int nums2=10;
    int results = num1+num2;
    System.out.println("Sum is " + result + " to test")
}

Console: Sum is 20 to test
```

## Reference and Primitive Types
Reference are on the Heap
Primitives are on the Stack
