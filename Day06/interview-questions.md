####  What are wrapper classes ?

- They are wrappers to primitive data types. They allow us to access primitives as objects.

####  Difference between boolean and Boolean ?

- boolean is a primitive type whereas Boolean is a class.

####  Explain Autoboxing ?

- Autoboxing is the automatic conversion that the Java compiler makes between the primitive types and their corresponding object wrapper classes

####  What are Wrapper Classes ? What are Primitive Wrapper Classes ?

- A wrapper class is any class which "wraps" or "encapsulates" the functionality of another class or component. A Wrapper Class that wraps or encapsulates the primitive data type is called Primitive Wrapper Class.

####  What Design pattern Wrapper Classes implement ?

- Adapter.

#### Comparable vs Comparator

- https://www.journaldev.com/780/comparable-and-comparator-in-java-example

#### What are some of the  java core libraries that are part of jre ?
  - Collections - java.util.*
  - jdbc        - java.sql.*
  - Threads     - java.lang.* // default package.
  - LocalDate   - java.time
  - Date -        java.util.*
  - file -        java.io  and java.nio.
  - Math        - java.lang.*

#### What are the basic interfaces of Java Collections Framework ?
  -  Java Collections Framework provides a well designed set of interfaces and classes that support operations on a collections of objects. The most basic interfaces that reside in the Java Collections Framework are:
  -  Collection, which represents a group of objects known as its elements.
  -  Set, which is a collection that cannot contain duplicate elements.
  -  List, which is an ordered collection and can contain duplicate elements.
  -  Map, which is an object that maps keys to values and cannot contain duplicate keys.

#### How do you check if two Strings are equal in Java?
  - There are two ways to check if two Strings are equal or not – using “==” operator or using equals method. When we use “==” operator, it checks for the value of String as well as the reference but in our programming, most of the time we are checking equality of String for value only. So we should use the equals method to check if two Strings are equal or not.
  There is another function equalsIgnoreCase that we can use to ignore case.

#### What is String Pool?
 - String Pool is a pool of Strings stored in Java heap memory. As String is a special class in Java and we can create String object using new operator as well as providing values in double quotes. String pool helps making String as an immutable object.

#### What is the benefit of Generics in Collections Framework?
   - Generics allow us to provide the type of Object that a collection can contain, so if you try to add any element of other type it throws compile time error. This avoids ClassCastException at Runtime because you will get the error at compilation. Also Generics make code clean since we don’t need to use casting and instanceof operator.
