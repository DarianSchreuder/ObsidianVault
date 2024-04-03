# Relationships(e.g Association)
2023-05-31 | 01:15
{Subject}:[[CMPG 211]]
{Section}:[[CMPG 211]]
{Tags}: #Programming #Java 
{Related}:

--- 
Association, aggregation, and composition are three different types of relationships that can exist between objects in object-oriented programming. These relationships define how objects are connected and interact with each other.

1. Association:
Association represents a relationship between two or more objects where each object has its own lifecycle, and there is no ownership or containment between them. It is a very generic relationship that can be of any type, such as a "uses," "has," or "knows" relationship.

Example: Consider a Car and a Driver. A car can have a driver associated with it, but the driver can also drive other cars. The Car and Driver objects are associated with each other, but neither object has ownership or control over the other.

2. Aggregation:
Aggregation is a specialized form of association where objects have a "whole" and "part" relationship. It is a stronger form of association that implies ownership. In aggregation, the "part" objects can exist independently of the "whole" object.

Example: A University and its Departments. A University consists of multiple departments, such as the Department of Computer Science, Department of Mathematics, etc. The University is the "whole" and the Departments are the "parts." If the University is dissolved, the Departments can still exist.

3. Composition:
Composition is also a form of association where objects have a "whole" and "part" relationship like aggregation. However, it is a stronger relationship where the "part" objects cannot exist independently of the "whole" object. The "part" objects are exclusive to the "whole" object, and their lifecycles are tightly coupled.

Example: A House and its Rooms. A House is composed of multiple rooms like a bedroom, living room, kitchen, etc. The Rooms are the "parts," and they cannot exist without the House. If the House is demolished, the Rooms cease to exist.

In summary, the key differences are:
- Association is a generic relationship between objects.
- Aggregation is a "whole" and "part" relationship where the "part" objects can exist independently.
- Composition is a "whole" and "part" relationship where the "part" objects cannot exist independently and have a tightly coupled lifecycle with the "whole" object.

Certainly! Here are examples of Association, Aggregation, and Composition in Java:

1. Association:
```java
class Car {
    private Driver driver;
    
    public void setDriver(Driver driver) {
        this.driver = driver;
    }
    
    // Other methods and attributes
}

class Driver {
    // Driver class implementation
}

// Usage:
Car car = new Car();
Driver driver = new Driver();
car.setDriver(driver);
```

In this example, the `Car` class is associated with the `Driver` class. The `Car` has a `Driver` associated with it, but the driver can also drive other cars. There is no ownership or containment relationship between them.

2. Aggregation:
```java
class University {
    private List<Department> departments;
    
    public University() {
        departments = new ArrayList<>();
    }
    
    public void addDepartment(Department department) {
        departments.add(department);
    }
    
    // Other methods and attributes
}

class Department {
    // Department class implementation
}

// Usage:
University university = new University();
Department csDepartment = new Department();
university.addDepartment(csDepartment);
```

In this example, the `University` class has an aggregation relationship with the `Department` class. The `University` consists of multiple `Department` objects, but the `Department` objects can exist independently of the `University` object.

3. Composition:
```java
class House {
    private List<Room> rooms;
    
    public House() {
        rooms = new ArrayList<>();
        rooms.add(new Room("Bedroom"));
        rooms.add(new Room("Living Room"));
        rooms.add(new Room("Kitchen"));
    }
    
    // Other methods and attributes
}

class Room {
    private String name;
    
    public Room(String name) {
        this.name = name;
    }
    
    // Room class implementation
}

// Usage:
House house = new House();
```

In this example, the `House` class has a composition relationship with the `Room` class. The `House` is composed of multiple `Room` objects (e.g., bedroom, living room, kitchen), and they cannot exist independently of the `House`. If the `House` is destroyed, the `Room` objects cease to exist.

These examples demonstrate the different types of relationships and how they can be implemented in Java.

--- 
{Efundi Lecture Notes}: [Relationships(e.g Association)]()