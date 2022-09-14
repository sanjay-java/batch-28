#### What is Inheritance
    Inheritance provides an object with the ability to acquire the fields and methods of another class, called base class. Inheritance provides re-usability of code and can be used to add additional features to an existing class, without modifying it.

#### Abstraction
    Abstraction is the process of separating ideas from specific instances and thus, develop classes in terms of their own functionality, instead of their implementation details. Java supports the creation and existence of abstract classes that expose interfaces, without including the actual implementation of all methods. The abstraction technique aims to separate the implementation details of a class from its behavior.

####  What is Encapsulation
        Encapsulation provides objects with the ability to hide their internal characteristics and behavior.
          Some of the advantages of using encapsulation are listed below:
            The internal state of every objected is protected by hiding its attributes.
            It increases usability and maintenance of code, because the behavior of an object can be independently changed or extended.
            It improves modularity by preventing objects to interact with each other, in an undesired way.

####  What is Polymorphism
        Polymorphism is the ability of an object to take on many forms.
        Compile Time Polymorphism - is a process in which an overloaded method is resolved at compile time.
        Runtime Polymorphism - is a process in which a call to an overridden method is resolved at runtime rather than compile-time


#### Differences between Abstraction and Encapsulation
    Abstraction and encapsulation are complementary concepts. On the one hand, abstraction focuses on the behavior of an object. On the other hand, encapsulation focuses on the implementation of an object’s behavior. Encapsulation is usually achieved by hiding information about the internal state of an object and thus, can be seen as a strategy used in order to provide abstraction.

#### Which class is the superclass of all classes?
    java.lang.Object is the root class for all the java classes and we don’t need to extend it.

#### Why Java doesn’t support multiple inheritance?
    Java doesn’t support multiple inheritance in classes because of “Diamond Problem”.
    However multiple inheritances are supported in interfaces. An interface can extend multiple interfaces because they just declare the methods and implementation will be present in the implementing class. So there is no issue of the diamond problem with interfaces.

#### What is an interface?
    Interfaces are core concepts of java programming language and used a lot not only in JDK but also java design patterns, most of the frameworks and tools. Interfaces provide a way to achieve abstraction in java and used to define the contract for the subclasses to implement.
    Interfaces are good for starting point to define Type and create top level hierarchy in our code. Since a java class can implements multiple interfaces, it’s better to use interfaces as super class in most of the cases. Read more at java interface.

#### What is an abstract class?
    Abstract classes are used in java to create a class with some default method implementation for subclasses. An abstract class can have an abstract method without the body and it can have methods with implementation also.
    abstract keyword is used to create a abstract class. Abstract classes can’t be instantiated and mostly used to provide base for sub-classes to extend and implement the abstract methods and override or use the implemented methods in abstract class. Read important points about abstract classes at java abstract class.

#### What is the difference between abstract class and interface?
    abstract keyword is used to create abstract class whereas interface is the keyword for interfaces.
    Abstract classes can have method implementations whereas interfaces can’t.

    A class can extend only one abstract class but it can implement multiple interfaces.

    We can run an abstract class if it has a main() method whereas we can’t run an interface.


#### Can an interface implement or extend another interface?
    Interfaces don’t implement another interface, they extend it. Since interfaces can’t have method implementations, there is no issue of diamond problem. That’s why we have multiple inheritances in interfaces i.e an interface can extend multiple interfaces.
    From Java 8 onwards, interfaces can have default method implementations. So to handle diamond problem when a common default method is present in multiple interfaces, it’s mandatory to provide implementation of the method in the class implementing them. For more details with examples, read Java 8 interface changes.


#### What is Marker interface?
    A marker interface is an empty interface without any method but used to force some functionality in implementing classes by Java. Some of the well known marker interfaces are Serializable and Cloneable.
