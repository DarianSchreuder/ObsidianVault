# ArrayList
2023-05-16 | 19:07
{Subject}:[[CMPG 211]]
{Section}:[[Array]]
{Tags}: #Programming 
{Related}:

--- 
In Java, `ArrayList` is a class that implements the `List` interface and provides a dynamic array-like data structure. It allows you to store and manipulate a collection of elements.

Here are some key points about `ArrayList` in Java:

1. Dynamic Size: Unlike regular arrays, `ArrayList` automatically grows and shrinks as elements are added or removed. You do not need to specify the size in advance.

2. Generic Type: `ArrayList` is a generic class, meaning you can specify the type of elements it will hold. For example, `ArrayList<Integer>` will only allow storing integer values.

3. Ordered Collection: `ArrayList` maintains the order of elements as they are added. The order of elements can be accessed and modified using indices.

4. Random Access: Elements in `ArrayList` can be accessed in constant time using their indices. This allows for efficient random access to elements.

5. Methods and Operations: `ArrayList` provides a wide range of methods to manipulate and access its elements. Some commonly used methods include `add()`, `get()`, `set()`, `remove()`, `size()`, and `contains()`.

Here's an example demonstrating the usage of `ArrayList` in Java:

```java
import java.util.ArrayList;

public class ArrayListExample {
    public static void main(String[] args) {
        // Creating an ArrayList of integers
        ArrayList<Integer> numbers = new ArrayList<>();

        // Adding elements to the ArrayList
        numbers.add(10);
        numbers.add(20);
        numbers.add(30);

        // Accessing elements by index
        System.out.println(numbers.get(0)); // Output: 10

        // Modifying an element
        numbers.set(1, 25);
        System.out.println(numbers); // Output: [10, 25, 30]

        // Removing an element by index
        numbers.remove(2);
        System.out.println(numbers); // Output: [10, 25]

        // Checking if an element exists
        System.out.println(numbers.contains(25)); // Output: true

        // Getting the size of the ArrayList
        System.out.println(numbers.size()); // Output: 2
    }
}
```

In this example, we create an `ArrayList` of integers, add elements, access elements using indices, modify elements, remove elements, check for the presence of an element, and obtain the size of the `ArrayList`.

--- 
{Efundi Lecture Notes}: [ArrayList]()