# Java\`s Excepion Hierarchy
2023-05-16 | 19:24
{Subject}:[[CMPG 211]]
{Section}:[[Exceptions]]
{Tags}: #Programming #Java 
{Related}:

--- 
In Java, exceptions are organized into a hierarchy of classes and interfaces that extend or implement one another. The root of the hierarchy is the `Throwable` class, which has two main subclasses: `Exception` and `Error`. Here's an overview of the Java Exceptions hierarchy:

1. Throwable:
   - `Throwable` is the root class of the exception hierarchy.
   - It provides the basic functionality for exceptions, including a message and a stack trace.
   - It has two main subclasses: `Exception` and `Error`.

2. Exception:
   - `Exception` is a subclass of `Throwable` and represents exceptional conditions that can be caught and handled.
   - It can further be divided into two categories: checked exceptions and unchecked exceptions.
   - Checked exceptions require explicit handling by the programmer through `try-catch` blocks or declaring them in method signatures using the `throws` keyword.
   - Unchecked exceptions, also known as runtime exceptions, do not require explicit handling.

3. Checked Exceptions:
   - Checked exceptions are exceptions that extend the `Exception` class and must be either caught or declared in the method signature using the `throws` keyword.
   - Some common checked exceptions include `IOException`, `SQLException`, and `ClassNotFoundException`.

4. Unchecked Exceptions (Runtime Exceptions):
   - Unchecked exceptions are exceptions that extend the `RuntimeException` class or one of its subclasses.
   - They do not require explicit handling by the programmer.
   - Some common runtime exceptions include `NullPointerException`, `ArrayIndexOutOfBoundsException`, and `ArithmeticException`.

5. Error:
   - `Error` is a subclass of `Throwable` and represents exceptional conditions that are typically beyond the control of the application.
   - Errors are usually severe and not meant to be caught or handled by application code.
   - Examples of errors include `OutOfMemoryError` and `StackOverflowError`.

By understanding the Java Exceptions hierarchy, you can effectively handle and manage exceptional conditions in your code by catching and handling specific exceptions, or allowing them to propagate up the call stack if appropriate.

Checked Exceptions:
- Checked exceptions are exceptions that are checked at compile time by the Java compiler.
- They represent exceptional conditions that a program might encounter and expects the developer to handle or declare in the method signature.
- Checked exceptions extend the `Exception` class (excluding its subclasses that extend `RuntimeException`).
- Examples of checked exceptions include `IOException`, `SQLException`, and `ClassNotFoundException`.
- To handle checked exceptions, you can use a `try-catch` block to catch the exception and provide appropriate error handling code, or you can declare the exception in the method signature using the `throws` keyword to indicate that the exception may be thrown by the method and should be handled by the calling code.

Unchecked Exceptions (Runtime Exceptions):
- Unchecked exceptions, also known as runtime exceptions, are exceptions that do not need to be checked at compile time.
- They extend the `RuntimeException` class or one of its subclasses.
- Unchecked exceptions represent programming errors or unexpected conditions that may occur at runtime, such as null references, array index out of bounds, or arithmetic errors.
- Unlike checked exceptions, there is no requirement to explicitly catch or declare unchecked exceptions.
- However, it is still possible to catch and handle unchecked exceptions using a `try-catch` block if desired.
- Common examples of unchecked exceptions include `NullPointerException`, `ArrayIndexOutOfBoundsException`, and `ArithmeticException`.

The distinction between checked and unchecked exceptions allows the developer to differentiate between exceptional conditions that are expected and require explicit handling (checked exceptions), and those that are typically programming errors or unexpected situations (unchecked exceptions).

--- 
{Efundi Lecture Notes}: [Java`s Excepion Hierarchy]()