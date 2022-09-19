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

#### What are the basic interfaces of Java Collections Framework?
     Collection is the root of the collection hierarchy. A collection represents a group of objects known as its elements. The Java platform doesn’t provide any direct implementations of this interface.

     Set is a collection that cannot contain duplicate elements. This interface models the mathematical set abstraction and is used to represent sets, such as the deck of cards.

     List is an ordered collection and can contain duplicate elements. You can access any element from its index. The list is more like an array with dynamic length.

   A Map is an object that maps keys to values. A map cannot contain duplicate keys: Each key can map to at most one value.

#### What is an Iterator?
       The Iterator interface provides methods to iterate over any Collection. We can get iterator instance from a Collection using iterator() method. Java Collection iterator provides a generic way for traversal through the elements of a collection. Iterators also allows the caller to remove elements from the underlying collection during the iteration.

#### What are different ways to iterate over a list?
     We can iterate over a list in two different ways – using iterator and using for-each loop.

#### What are similarities and difference between ArrayList and Vector?
   - similarities
       Both are index based and backed up by an array internally.
       Both maintains the order of insertion and we can get the elements in the order of insertion.
       The iterator implementations of ArrayList and Vector both are fail-fast by design.
       ArrayList and Vector both allows null values and random access to element using index number.
   - differences
       Vector is synchronized whereas ArrayList is not synchronized. However if you are looking for modification of list while iterating, you should use CopyOnWriteArrayList.
       ArrayList is faster than Vector because it doesn’t have any overhead because of synchronization.
       ArrayList is more versatile because we can get synchronized list or read-only list from it easily using Collections utility class.

#### What is difference between Array and ArrayList? When will you use Array over ArrayList?
     -   Arrays can contain primitive or Objects whereas ArrayList can contain only Objects.
         Arrays are fixed-size whereas ArrayList size is dynamic.
         Arrays don’t provide a lot of features like ArrayList, such as addAll, removeAll, iterator, etc.

         Although ArrayList is the obvious choice when we work on the list, there are a few times when an array is good to use.

         If the size of list is fixed and mostly used to store and traverse them.
         For list of primitive data types, although Collections use autoboxing to reduce the coding effort but still it makes them slow when working on fixed size primitive data types.

#### What is difference between ArrayList and LinkedList?

     - ArrayList and LinkedList both implement List interface but there are some differences between them.

       ArrayList is an index based data structure backed by Array, so it provides random access to its elements with performance as O(1) but LinkedList stores data as list of nodes where every node is linked to its previous and next node. So even though there is a method to get the element using index, internally it traverse from start to reach at the index node and then return the element, so performance is O(n) that is slower than ArrayList.

       Insertion, addition or removal of an element is faster in LinkedList compared to ArrayList because there is no concept of resizing array or updating index when element is added in middle.

       LinkedList consumes more memory than ArrayList because every node in LinkedList stores reference of previous and next elements.

#### What is Big-O notation? Give some examples?
     The Big-O notation describes the performance of an algorithm in terms of the number of elements in a data structure. Since Collection classes are data structures, we usually tend to use Big-O notation to chose the collection implementation to use based on time, memory and performance.

       Example 1: ArrayList get(index i) is a constant-time operation and doesn’t depend on the number of elements in the list. So its performance in Big-O notation is O(1).

       Example 2: A linear search on array or list performance is O(n) because we need to search through entire list of elements to find the element.

#### What is the difference between List and set

       The main difference between the List and Set interface in Java is that List allows duplicates while Set doesn't allow duplicates. All implementation of Set honor this contract.

       Lists maintains insertion order of elements. Set is an unordered collection, you get no guarantee on which order element will be stored.

#### Difference between HashSet vs TreeSet
       HashSet is Implemented using a hash table. Elements are not ordered. Where as, TreeSet is implemented using a tree structure. The elements in a set are sorted.

       HashSet is faster than TreeSet and should be preferred choice if sorting of element is not required.

       HashSet allows null object but TreeSet doesn't allow null Object and throw NullPointerException
