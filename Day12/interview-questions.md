https://www.baeldung.com/java-8-interview-questions

####  What are new features which got introduced in Java 8?
  There are lots of new features which were added in Java 8. Here is the list of important features:

  - Lambda Expression
  - Stream API
  - Default methods in the interface
  - Functional Interface
  - Optional
  - Method reference
  - Date API
  - Nashorn, JavaScript Engine

#### What are main advantages of using Java 8?
  -  More compact code
  - Less boiler plate code
  - More readable and reusable code
  - More testable code
  - Parallel operations

#### What is lambda expression?
  - Lambda expression is anonymous function which have set of parameters and a lambda (->) and a function body.

####  Can you explain the syntax of Lambda expression?
  -  Argument list or parameters - Lambda expression can have zero or more arguments.
  - Array token (->) or arrow symbol -
  - Body
    - Body can have expression or statements.
    - If there is only one statement in body, curly brace is not needed and return type of the anonymous function is same as of  body expression
    - If there are more than one statements, then it should be in curly braces and return type of anonymous function is same as value return from code block, void if nothing is returned.

#### What are functional interfaces?
  - Functional interfaces are those interfaces which can have only one abstract method. It can have static method, default methods or can override Object’s class methods. Where an instance of such an interface is required, a Lambda Expression can be used instead. More formally put: Functional interfaces provide target types for lambda expressions and method references.

####  Describe Some of the Functional Interfaces in the Standard Library
  There are a lot of functional interfaces in the java.util.function package. The more common ones include, but are not limited to:

  Function – it takes one argument and returns a result
  Consumer – it takes one argument and returns no result (represents a side effect)
  Supplier – it takes no arguments and returns a result
  Predicate – it takes one argument and returns a boolean
  BiFunction – it takes two arguments and returns a result

####  How Can you create your own functional interface?
  - you can create your own functional interface. Java can implicitly identify functional interface but you can also annotate it with @FunctionalInterface.

#### What is method reference in java 8?
  - Method reference is used refer method of functional interface. It is nothing but compact way of lambda expression.You can simply replace lambda expression with method reference.
  Syntax:
  class::methodname
#### What is Optional? Why and how can you use it?
  - Java 8 has introduced new class Called Optional. This class is basically introduced to avoid NullPointerException in java. Optional class encapsulates optional value which is either present or not. It is a wrapper around object and can be use to avoid NullPointerExceptions.

#### What is Type Inference?
  - Type inference helps the compiler determine the argument types by looking at each method invocation and corresponding declaration.

#### What is a stream, and how does it differ from a collection?
  - A stream is an iterator whose function is to accept a set of actions and apply them to each of the elements it contains. A stream represents an object sequence from a collection or other source that supports aggregate operations. Unlike collections, iteration logic implements inside the stream. Also, streams are inherently lazily loaded and processed, unlike collections.

#### What is a SAM Interface?

  - Java 8 has introduced the concept of FunctionalInterface that can have only one abstract method. Since these Interfaces specify only one abstract method, they are sometimes called as SAM Interfaces. SAM stands for “Single Abstract Method”.

#### Why do we require the Stream API?

  - Stream API is a new feature added in Java 8. It is a special class that is used for processing objects from a source such as Collection.
  We require the Stream API because,
    - It supports aggregate operations which makes the processing simple.
    - It supports Functional-Style programming.
    - It does faster processing. Hence, it is apt for better performance.
    - It allows parallel operations.
