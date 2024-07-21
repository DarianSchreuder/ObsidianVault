# Abstract in Java
2023-04-13 | 20:18
{Subject}:[[CMPG 211]]
{Tags}: #Programming #Java #ComputerScience 
{Related}:[[Interfaces in Java]]

--- 
In Java, the `abstract` keyword is used to define abstract classes and abstract methods.

1. Abstract Classes:
   - An abstract class is a class that cannot be instantiated and serves as a blueprint for other classes.
   - It can contain both abstract and non-abstract methods.
   - Abstract classes may have constructors, instance variables, and non-abstract methods with implementations.
   - To declare an abstract class, use the `abstract` keyword before the class declaration.
   
   ```java
   public abstract class AbstractClass {
       // Abstract method declaration
       public abstract void abstractMethod();
   
       // Non-abstract method with implementation
       public void nonAbstractMethod() {
           // Implementation code
       }
   }
   ```

2. Abstract Methods:
   - An abstract method is a method without an implementation, defined using the `abstract` keyword.
   - Abstract methods are declared in an abstract class but do not provide an implementation.
   - Any class that extends the abstract class must provide an implementation for all the abstract methods.
   
   ```java
   public abstract class AbstractClass {
       public abstract void abstractMethod();
   }
   ```

To use abstract classes and methods in Java, follow these steps:

1. Extend an Abstract Class:
   - To use an abstract class, create a new class that extends the abstract class using the `extends` keyword.
   - Implement the abstract methods defined in the abstract class.
   
   ```java
   public class ConcreteClass extends AbstractClass {
       public void abstractMethod() {
           // Implementation code
       }
   }
   ```

2. Implement Abstract Methods:
   - When a class extends an abstract class, it must provide an implementation for all the abstract methods inherited from the abstract class.
   - Use the `@Override` annotation to ensure that you are correctly overriding the abstract method.
   
   ```java
   public class ConcreteClass extends AbstractClass {
       @Override
       public void abstractMethod() {
           // Implementation code
       }
   }
   ```

Abstract classes and methods are useful when you want to define common behavior and leave certain methods to be implemented by subclasses. They allow for code reusability and provide a level of abstraction in your Java programs.
--- 
{Efundi Lecture Notes}: [Object-Oriented Problem Solving](https://efundi.nwu.ac.za/access/content/group/94d75855-14f5-4f6e-8f10-ad685dbe113c/Textbook/jjj-CMPG211_Version20230221b.pdf)