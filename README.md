# OOPs-In-Java
OOPS CONCEPT IN JAVA

Object-Oriented Programming is a methodology or paradigm to design a program using classes and objects. It simplifies software development and maintenance by providing some concepts:
•	Object
•	Class
•	Inheritance
•	Polymorphism
•	Abstraction
•	Encapsulation
Object: object is called as run time entity that has state and behavior. It has three characteristics:
State: represents the data (value) of an object.
Behavior: represents the behavior (functionality) of an object such as deposit, withdraw, etc.
Identity: An object identity is typically implemented via a unique ID. The value of the ID is not visible to the external user. However, it is used internally by the JVM to identify each object uniquely.
Class: A class is a collection of members and member-function, from which objects are created. So, an object is the instance(result) of a class.
A class in Java can contain:
•	Fields
•	Methods
•	Constructors
•	Blocks
•	Nested class and interface 
Inheritance: Inheritance is a mechanism where child class acquires all the properties from its parent class. The main motto of inheritance is to reduce the redundancy of the code, you inherit from an existing class, you can reuse methods and fields of the parent class. Moreover, you can add new methods and fields in your current class also. 
•	Single inheritance
•	Multilevel inheritance
•	Hierarchical inheritance
•	Multiple inheritance
•	Hybrid Inheritance
Polymorphism: Polymorphism in Java is the ability of an object to take many forms. To simply put, polymorphism in java allows us to perform the same action in many different ways. Any Java object that can pass more than one IS-A test is  considered to be polymorphic and in java, all the java objects are polymorphic as it has passed the IS-A test for their own type and for the class Object. There are two types of polymorphism in java: compile-time polymorphism and runtime polymorphism. There are two types of polymorphism 
•	Method Overloading.
•	Method overriding.
Method Overloading: Method overloading is defined as a process that can create multiple methods of the same name in the same class, and all the methods work in different ways. Method overloading occurs when there is more than one method of the same name in the class.
               class ramki {
  public void ram() {
    System.out.println("Find area ");
  }
public void ram(int r) {
    System.out.println("Circle area = "+3.14*r*r);

  }
}
class Main {
  public static void main(String[] args) {
    ramki poly = new ramki();  // Create a Shapes object
     
    poly.area();
    poly.area(5);
     
  }
}

Method Overriding: Method overriding is defined as a process when the subclass or a child class has the same method as declared in the parent class. Polymorphism in java can be classified into two types:

Static or Compile-Time Polymorphism:  Compile-Time polymorphism in java is also known as Static Polymorphism. In this process, the call to the method is resolved at compile-time. Compile-Time polymorphism is achieved through Method Overloading. This type of polymorphism can also be achieved through Operator Overloading. However, Java does not support Operator Overloading.
Dynamic / Runtime Polymorphism: Runtime polymorphism in java is also known as Dynamic Binding or Dynamic Method Dispatch. In this process, the call to an overridden method is resolved dynamically at runtime rather than at compile-time. Runtime polymorphism is achieved through Method Overriding.
Abstraction: Abstraction is a process of hiding the implementation details and showing only functionality to the user. Another way, it shows only essential things to the user and hides the internal details, for example, sending SMS where you type the text and send the message. You don't know the internal processing about the message deliver. This can be achieved by using abstract keyword before the   name of the class or method.

abstract class Bike{  
  abstract void run();  
}  
class Honda4 extends Bike{  
void run(){System.out.println("running safely");}  
public static void main(String args[]){  
 Bike obj = new Honda4();  
 obj.run();  
}  
}  
Encapsulation:  Encapsulation in Java is a process of wrapping code and data together into a single unit, for example, a capsule which is mixed of several medicines. We can create a fully encapsulated class in Java by making all the data members of the class private. Now we can use setter and getter methods to set and get the data in it.
