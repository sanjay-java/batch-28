#### What is String Pool?
     As the name suggests, String Pool is a pool of Strings stored in Java heap memory. We know that String is a special class in Java and we can create String object using new operator as well as providing values in double quotes.

#### What are different ways to create String Object?
    We can create String object using new operator like any normal java class or we can use double quotes to create a String object. There are several constructors available in String class to get String from char array, byte array, StringBuffer and StringBuilder.

#### Read and practice one or two sorting algorithms
     https://stackabuse.com/sorting-algorithms-in-java/

#### How do you check the equality of two arrays in java? OR How do you compare the two arrays in java?
    You can use Arrays.equals() method to compare one dimensional arrays and to compare multidimensional arrays, use Arrays.deepEquals() method.

#### Can you change the size of the array once you define it? OR Can you insert or delete the elements after creating an array?
    No. You can’t change the size of the array once you define it. You can not insert or delete the elements after creating an array. Only you can do is change the value of the elements.

#### What is final keyword?
    The final keyword is used with Class to make sure no other class can extend it. For example, the String class is final and we can’t extend it.
    We can use the final keyword with methods to make sure child classes can’t override it.
    Java’s final keyword can be used with variables to make sure that it can be assigned only once. However the state of the variable can be changed, for example, we can assign a final variable to an object only once but the object variables can change later on.
    Java interface variables are by default final and static.

#### What is static keyword?
    static keyword can be used with class-level variables to make it global i.e all the objects will share the same variable.
    static keyword can be used with methods also. A static method can access only static variables of class and invoke only static methods of the class.


#### What is Java Package and which package is imported by default?
     Java package is the mechanism to organize the java classes by grouping them. The grouping logic can be based on functionality or modules based. A java class fully classified name contains package and class name. For example, java.lang.Object is the fully classified name of Object class that is part of java.lang package.

    java.lang package is imported by default and we don’t need to import any class from this package explicitly.


#### What is the importance of main method in Java?
      main() method is the entry point of any standalone java application. The syntax of main method is public static void main(String args[]).
      Java’s main method is public and static so that Java runtime can access it without initializing the class. The input parameter is an array of String through which we can pass runtime arguments to the java program. Check this post to learn how to compile and run java program.

#### What is overloading and overriding in java?
      When we have more than one method with the same name in a single class but the arguments are different, then it is called method overloading.
      The overriding concept comes in picture with inheritance when we have two methods with the same signature, one in the parent class and another in child class. We can use @Override annotation in the child class overridden method to make sure if the parent class method is changed, so as child class.


#### Can we overload main method?
      Yes, we can have multiple methods with name “main” in a single class. However if we run the class, java runtime environment will look for main method with syntax as public static void main(String args[]).

#### Can we have multiple public classes in a java source file?
      We can’t have more than one public class in a single java source file. A single source file can have multiple classes that are not public.
