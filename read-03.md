# Reading Notes 03

[Java Primitives vs Objects](https://www.baeldung.com/java-primitives-vs-objects)



## Files Primitives File I/O

int, boolean vs Integer, Boolean -- wrapper classes are immutable and final

`Integer j = 1;          // autoboxing
int i = new Integer(1); // unboxing`


-    boolean – 1 bit
-    byte – 8 bits
-    short, char – 16 bits
-    int, float – 32 bits
-    long, double – 64 bits

These live on stack, hence access is fast.

Reference types, being objects, live on heap, therefore are slow to access.

'single-element arrays of primitive types are almost always more expensive (except for long and double) than the corresponding reference type.'

#### the objects in Java are slower and have a bigger memory impact than their primitive analogs.


## Exceptions
In Java, an exception is an event that disrupts the normal flow of the program. It is an object which is thrown at runtime.

What is the difference between error and exception?
Some of the examples of errors are system crash error and out of memory error. Errors mostly occur at runtime that's they belong to an unchecked type. Exceptions are the problems which can occur at runtime and compile time. ... Exceptions are divided into two categories such as checked exceptions and unchecked exceptions.

![sd.lm](https://simplesnippets.tech/wp-content/uploads/2018/05/java-exception-handling-class-hierarchy-diagram.jpg)

A program can catch exceptions by using a combination of the try, catch, and finally blocks.

The try block identifies a block of code in which an exception can occur.
The catch block identifies a block of code, known as an exception handler, that can handle a particular type of exception.
The finally block identifies a block of code that is guaranteed to execute, and is the right place to close files, recover resources, and otherwise clean up after the code enclosed in the try block.
The try statement should contain at least one catch block or a finally block and may have multiple catch blocks.


# Scanning
![sdl](https://techvidvan.com/tutorials/wp-content/uploads/sites/2/2020/06/Scanner-Class-in-java-1200x720.jpg)

Scanner is a class in java. util package used for obtaining the input of the primitive types like int, double, etc. and strings.

It is the easiest way to read input in a Java program, though not very efficient if you want an input method for scenarios where time is a constraint like in competitive programming.
