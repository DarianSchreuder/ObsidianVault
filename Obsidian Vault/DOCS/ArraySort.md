# ArraySort
2023-05-16 | 19:10
{Subject}:[[CMPG 211]]
{Section}:[[Array]]
{Tags}: #Programming #Java #ComputerScience 
{Related}:

--- 
The `Arrays.sort()` method in Java is used to sort arrays in ascending order. It is part of the `java.util.Arrays` class and provides an efficient implementation of the sorting algorithm.

Here's a detailed explanation of `Arrays.sort()`:

1. Sorting Arrays of Primitive Types:
   - When sorting arrays of primitive types (e.g., `int`, `char`, etc.), the `Arrays.sort()` method uses a variant of the quicksort algorithm.
   - The syntax for sorting an array of primitive types is as follows:

   ```java
   int[] arr = {5, 2, 8, 1, 9};
   Arrays.sort(arr);
   ```

   After the above code is executed, the `arr` array will be sorted in ascending order: `{1, 2, 5, 8, 9}`.

2. Sorting Arrays of Objects Implementing `Comparable`:
   - If you have an array of objects that implement the `Comparable` interface, you can use `Arrays.sort()` to sort them based on their natural order.
   - The `Comparable` interface defines the `compareTo()` method, which provides the comparison logic for determining the ordering of objects.
   - The syntax for sorting an array of objects implementing `Comparable` is as follows:

   ```java
   String[] names = {"John", "Alice", "Bob", "David"};
   Arrays.sort(names);
   ```

   After the above code is executed, the `names` array will be sorted in alphabetical order: `{"Alice", "Bob", "David", "John"}`.

3. Sorting Arrays of Objects with Custom Comparison using `Comparator`:
   - If you have an array of objects that do not implement `Comparable`, you can use the overloaded version of `Arrays.sort()` that accepts a custom `Comparator`.
   - A `Comparator` is an interface that defines a comparison logic separate from the objects being compared.
   - You need to create a class implementing the `Comparator` interface and provide the comparison logic in the `compare()` method.
   - The syntax for sorting an array of objects using a custom `Comparator` is as follows:

   ```java
   Person[] people = {person1, person2, person3};
   Arrays.sort(people, new CustomComparator());
   ```

   In the above example, `person1`, `person2`, and `person3` are instances of a custom `Person` class, and `CustomComparator` is a class implementing the `Comparator` interface with the custom comparison logic.

   The `compare()` method in the `CustomComparator` class would look like this:

   ```java
   public class CustomComparator implements Comparator<Person> {
       @Override
       public int compare(Person p1, Person p2) {
           // Custom comparison logic
           // Return a negative value if p1 should come before p2
           // Return a positive value if p1 should come after p2
           // Return 0 if p1 and p2 are considered equal in ordering
       }
   }
   ```

   The `Arrays.sort()` method will use the `compare()` method of the `CustomComparator` class to determine the ordering of objects in the `people` array.

These are the different ways you can use `Arrays.sort()` to sort arrays in Java, either using the natural order defined by `Comparable` or a custom `Comparator`.

--- 
{Efundi Lecture Notes}: [ArraySort]()