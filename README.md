# coreJavaReferenceNote

Let's dive into the detailed notes for each day, starting with Day 1:

### **Day 1: Introduction to Java**

#### Overview of Java
- **Java** is a high-level, class-based, object-oriented programming language.
- It is designed to have as few implementation dependencies as possible, making it platform-independent due to the Java Virtual Machine (JVM).
- Java is widely used for building enterprise-scale applications, Android apps, web applications, and more.

#### Features of Java
1. **Simple**: Easy to learn with a syntax similar to C++ but simpler.
2. **Object-Oriented**: Everything is represented as objects, promoting reusability and modularity.
3. **Platform-Independent**: Write Once, Run Anywhere (WORA); Java code is compiled into bytecode which can be executed on any system with a JVM.
4. **Secure**: Java has a strong emphasis on security, with features like the Java sandbox for running untrusted code.
5. **Robust**: Strong memory management, exception handling, and garbage collection.
6. **Multithreaded**: Supports concurrent execution of two or more threads.
7. **Portable**: The Java bytecode is platform-independent and can be run on any device with the JVM.
8. **Dynamic**: Supports dynamic linking and loading of classes.

#### Java Development Kit (JDK), Java Runtime Environment (JRE), and Java Virtual Machine (JVM)
- **JDK**: A full-featured software development kit for Java, including JRE, an interpreter/loader (Java), a compiler (javac), an archiver (jar), a documentation generator (Javadoc), and other tools.
- **JRE**: The Java Runtime Environment is the part of the Java Development Kit that contains all the tools needed to run Java applications, including the JVM and standard libraries.
- **JVM**: The Java Virtual Machine is an abstract computing machine that enables your computer to run a Java program. It converts Java bytecode into machine-specific code.

---

### **Day 2: Setting Up the Environment**

#### Installing JDK
1. Download the latest JDK from [Oracle's official website](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html) or [OpenJDK](https://jdk.java.net/).
2. Follow the installation instructions specific to your operating system (Windows, macOS, Linux).

#### Setting up an Integrated Development Environment (IDE)
- Popular IDEs for Java development include IntelliJ IDEA, Eclipse, and NetBeans.
- **IntelliJ IDEA**: 
  - Download from [JetBrains](https://www.jetbrains.com/idea/download/).
  - Follow the installation process and set up the JDK path in the IDE settings.

#### Writing and Running Your First Java Program
1. **Creating a Java Project**:
   - In your IDE, create a new Java project.
   - Set the project SDK to the installed JDK version.

2. **Writing a Simple Java Program**:
   ```java
   public class HelloWorld {
       public static void main(String[] args) {
           System.out.println("Hello, World!");
       }
   }
   ```
3. **Compiling and Running the Program**:
   - In the IDE, compile the program (usually with a 'Build' or 'Compile' button).
   - Run the program (usually with a 'Run' button).

---

### **Day 3: Basic Syntax and Data Types**

#### Structure of a Java Program
- **Class Declaration**: Defines a new class.
- **Main Method**: The entry point of any Java program.
- **Statements**: Code to be executed.

#### Variables, Data Types, and Literals
- **Variables**: Containers for storing data values. Example: `int number = 10;`
- **Data Types**:
  - **Primitive Data Types**: byte, short, int, long, float, double, char, boolean.
  - **Non-Primitive Data Types**: Strings, Arrays, Classes, etc.
- **Literals**: Fixed values assigned to variables, e.g., `int num = 100;`, `"Hello"`.

#### Naming Conventions
- **Classes**: PascalCase (e.g., `MyClass`)
- **Methods and Variables**: camelCase (e.g., `myMethod`, `myVariable`)
- **Constants**: UPPER_CASE (e.g., `PI_VALUE`)

---

### **Day 4: Operators and Expressions**

#### Types of Operators
1. **Arithmetic Operators**: `+`, `-`, `*`, `/`, `%`
2. **Relational Operators**: `==`, `!=`, `>`, `<`, `>=`, `<=`
3. **Logical Operators**: `&&`, `||`, `!`
4. **Bitwise Operators**: `&`, `|`, `^`, `~`, `<<`, `>>`, `>>>`
5. **Assignment Operators**: `=`, `+=`, `-=`, `*=`, `/=`, `%=`
6. **Unary Operators**: `+`, `-`, `++`, `--`, `!`

#### Operator Precedence
- Determines the order in which operators are evaluated in expressions.
- Example: `int result = 10 + 3 * 5; // result is 25`

---

### **Day 5: Control Flow Statements**

#### If-Else Statements
- **Syntax**:
  ```java
  if (condition) {
      // code to be executed if condition is true
  } else if (anotherCondition) {
      // code to be executed if anotherCondition is true
  } else {
      // code to be executed if all conditions are false
  }
  ```

#### Switch-Case
- **Syntax**:
  ```java
  switch (variable) {
      case value1:
          // code to be executed if variable == value1
          break;
      case value2:
          // code to be executed if variable == value2
          break;
      // more cases...
      default:
          // code to be executed if no cases match
  }
  ```

---

### **Day 6: Loops**

#### For Loop
- **Syntax**:
  ```java
  for (initialization; condition; update) {
      // code block to be executed
  }
  ```

#### While Loop
- **Syntax**:
  ```java
  while (condition) {
      // code block to be executed
  }
  ```

#### Do-While Loop
- **Syntax**:
  ```java
  do {
      // code block to be executed
  } while (condition);
  ```

#### Break and Continue Statements
- **Break**: Exits the loop prematurely.
- **Continue**: Skips the current iteration and continues with the next iteration.

---

### **Day 7: Understanding Arrays**

#### Declaring and Initializing Arrays
- **Single-dimensional array**:
  ```java
  int[] numbers = new int[5];
  int[] numbers = {1, 2, 3, 4, 5};
  ```
- **Multi-dimensional array**:
  ```java
  int[][] matrix = new int[3][3];
  int[][] matrix = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
  ```

#### Array Operations and Iteration
- Accessing elements: `numbers[0]`
- Iterating through an array:
  ```java
  for (int i = 0; i < numbers.length; i++) {
      System.out.println(numbers[i]);
  }
  ```

---

### **Day 8: Introduction to OOP**

#### Principles of OOP
1. **Encapsulation**: Bundling the data (attributes) and methods (functions) that operate on the data into a single unit, known as a class.
2. **Inheritance**: Mechanism where one class acquires the properties and behaviors of another class.
3. **Polymorphism**: Ability of a method to do different things based on the object it is acting upon.
4. **Abstraction**: Hiding the complex implementation details and showing only the essential features.

#### Classes and Objects
- **Class**: A blueprint for creating objects. It defines a datatype by bundling data and methods that work on the data into one single unit.
- **Object**: An instance of a class. It is created using the `new` keyword.

---

### **Day 9: Methods and Constructors**

#### Method Declaration and Invocation
- **Method Declaration**:
  ```java
  public int add(int a, int b) {
      return a + b;
  }
  ```
- **Method Invocation**:
  ```java
  MyClass obj = new MyClass();
  int sum = obj.add(5, 3);
  ```

#### Method Overloading
- Methods with the same name but different parameter lists.
  ```java
  public int add(int a, int b) {
      return a + b;
  }

  public double add(double a, double b) {
      return a + b;
  }
  ```

#### Constructors and Constructor Overloading
- **Constructor**: A special method used to initialize objects. It is called when an object of a class is created.
  ```java
  public MyClass() {
      // constructor body
  }
  ```
- **Constructor Overloading**: Multiple constructors with different parameter lists.

---

### **Day 10: Inheritance**

#### Types of Inheritance in Java
1. **Single Inheritance**: A class inherits from one superclass.
2. **Multilevel Inheritance**: A class is derived from another derived class.


3. **Hierarchical Inheritance**: Multiple classes inherit from one superclass.

#### The `super` Keyword
- Used to refer to the immediate parent class object.
- **Accessing parent class constructor**:
  ```java
  super();
  ```
- **Accessing parent class methods**:
  ```java
  super.methodName();
  ```

#### Method Overriding
- Redefining a superclass method in a subclass.
  ```java
  @Override
  public void display() {
      // overridden method body
  }
  ```

---

### **Day 11: Polymorphism**

#### Compile-time Polymorphism (Method Overloading)
- Same method name, different parameter lists.

#### Runtime Polymorphism (Method Overriding)
- Method implementation is determined at runtime.

---

### **Day 12: Abstraction and Interfaces**

#### Abstract Classes and Methods
- **Abstract Class**: A class that cannot be instantiated and may contain abstract methods.
  ```java
  public abstract class Animal {
      public abstract void sound();
  }
  ```

- **Abstract Method**: A method without a body, meant to be overridden in subclasses.
  ```java
  public abstract void sound();
  ```

#### Interfaces
- A reference type in Java, similar to a class, that can contain only constants, method signatures, default methods, static methods, and nested types.
  ```java
  public interface Animal {
      void sound();
  }
  ```

- **Implementing Interfaces**:
  ```java
  public class Dog implements Animal {
      public void sound() {
          System.out.println("Woof");
      }
  }
  ```

---

### **Day 13: Encapsulation**

#### Access Modifiers
1. **Private**: Accessible only within the same class.
2. **Default**: Accessible within the same package.
3. **Protected**: Accessible within the same package and by subclasses.
4. **Public**: Accessible from anywhere.

#### Getters and Setters
- Methods used to access and modify private fields.
  ```java
  public class Person {
      private String name;

      public String getName() {
          return name;
      }

      public void setName(String name) {
          this.name = name;
      }
  }
  ```

---

### **Day 14: Packages and Access Control**

#### Creating and Using Packages
- **Package**: A namespace that organizes a set of related classes and interfaces.
  ```java
  package com.example;
  ```

- **Using Packages**:
  - To use classes from another package, use the `import` statement.
  ```java
  import com.example.MyClass;
  ```

#### Import Statements
- **Single Type Import**:
  ```java
  import java.util.List;
  ```
- **On-Demand Import**:
  ```java
  import java.util.*;
  ```

#### Access Control within Packages
- Classes in the same package have default access and can access each other's package-private members.

---

### **Day 15: String Handling**

#### String Class and Methods
- Strings are immutable objects in Java.
- Common methods:
  - `length()`, `charAt()`, `substring()`, `equals()`, `compareTo()`, `toLowerCase()`, `toUpperCase()`, `trim()`, `replace()`, `split()`

#### StringBuilder and StringBuffer Classes
- **StringBuilder**: Mutable sequence of characters, not synchronized.
  ```java
  StringBuilder sb = new StringBuilder("Hello");
  sb.append(" World");
  ```

- **StringBuffer**: Synchronized version of StringBuilder.
  ```java
  StringBuffer sbf = new StringBuffer("Hello");
  sbf.append(" World");
  ```

---

### **Day 16: Exception Handling**

#### Types of Exceptions
1. **Checked Exceptions**: Exceptions that are checked at compile-time.
2. **Unchecked Exceptions**: Exceptions that are checked at runtime.

#### Try-Catch Block
- Handling exceptions using try-catch.
  ```java
  try {
      // code that may throw an exception
  } catch (ExceptionType e) {
      // handling code
  }
  ```

#### Finally Block
- A block that executes regardless of whether an exception is thrown or not.
  ```java
  finally {
      // cleanup code
  }
  ```

#### Throw and Throws Keywords
- **Throw**: Used to explicitly throw an exception.
  ```java
  throw new Exception("Error occurred");
  ```

- **Throws**: Indicates that a method may throw certain exceptions.
  ```java
  public void myMethod() throws IOException {
      // method code
  }
  ```

#### Custom Exceptions
- Creating your own exception classes.
  ```java
  public class CustomException extends Exception {
      public CustomException(String message) {
          super(message);
      }
  }
  ```

---

### **Day 17: Collections Framework**

#### Introduction to Collections
- **Collections**: Framework that provides an architecture to store and manipulate a group of objects.

#### List Interface
- **ArrayList**: Dynamic array.
- **LinkedList**: Doubly-linked list implementation.

#### Set Interface
- **HashSet**: Unordered, no duplicates.
- **TreeSet**: Sorted, no duplicates.

#### Map Interface
- **HashMap**: Key-value pairs, unordered.
- **TreeMap**: Key-value pairs, sorted.

---

### **Day 18: Generics**

#### Introduction to Generics
- Generics provide type safety and allow for code reusability.

#### Generic Classes and Methods
- **Generic Class**:
  ```java
  public class Box<T> {
      private T item;

      public void setItem(T item) {
          this.item = item;
      }

      public T getItem() {
          return item;
      }
  }
  ```

- **Generic Method**:
  ```java
  public <T> void printArray(T[] array) {
      for (T item : array) {
          System.out.println(item);
      }
  }
  ```

#### Bounded Type Parameters
- Restricting the types that can be used as generic arguments.
  ```java
  public <T extends Number> void printNumber(T number) {
      System.out.println(number);
  }
  ```

---

### **Day 19: I/O Streams**

#### File Handling in Java
- **File** class: Represents a file or directory path.
  ```java
  File file = new File("filename.txt");
  ```

#### Byte Streams and Character Streams
- **Byte Streams**: For binary data (e.g., `FileInputStream`, `FileOutputStream`).
- **Character Streams**: For character data (e.g., `FileReader`, `FileWriter`).

#### FileReader and FileWriter
- **FileReader**:
  ```java
  FileReader fr = new FileReader("file.txt");
  int i;
  while ((i = fr.read()) != -1) {
      System.out.print((char) i);
  }
  fr.close();
  ```

- **FileWriter**:
  ```java
  FileWriter fw = new FileWriter("file.txt");
  fw.write("Hello, World!");
  fw.close();
  ```

#### BufferedReader and BufferedWriter
- **BufferedReader**: For reading text from a character-input stream.
  ```java
  BufferedReader br = new BufferedReader(new FileReader("file.txt"));
  String line;
  while ((line = br.readLine()) != null) {
      System.out.println(line);
  }
  br.close();
  ```

- **BufferedWriter**: For writing text to a character-output stream.
  ```java
  BufferedWriter bw = new BufferedWriter(new FileWriter("file.txt"));
  bw.write("Hello, World!");
  bw.close();
  ```

---

### **Day 20: Multithreading Basics**

#### Introduction to Multithreading
- **Multithreading**: A process of executing multiple threads simultaneously.

#### Creating and Starting Threads
1. **By Extending the Thread Class**:
   ```java
   public class MyThread extends Thread {
       public void run() {
           System.out.println("Thread is running.");
       }
   }

   MyThread thread = new MyThread();
   thread.start();
   ```

2. **By Implementing the Runnable Interface**:
   ```java
   public class MyRunnable implements Runnable {
       public void run() {
           System.out.println("Thread is running.");
       }
   }

   MyRunnable runnable = new MyRunnable();
   Thread thread = new Thread(runnable);
   thread.start();
   ```

#### Thread Lifecycle
- **New**: A thread is in this state when it is created but not yet started.
- **Runnable**: A thread is in this state after calling the start() method but before it is selected to run by the thread scheduler.
- **Blocked**: A thread that is blocked waiting for a monitor lock.
- **Waiting**: A thread that is waiting indefinitely for another thread to perform a particular action.
- **Timed Waiting**: A thread that is waiting for another thread to perform a particular action for a specified waiting time.
- **Terminated**: A thread that has exited.

#### Synchronization
- Used to control the access of multiple threads to shared resources.
  ```java
  synchronized void synchronizedMethod() {
      // synchronized code
  }
  ```

---

### **Day 21: Advanced Multithreading**

#### Inter-thread Communication
- **wait()**: Causes the current thread to wait until another thread invokes the notify() or notifyAll() methods.
- **notify()**: Wakes up a single thread that is waiting on this object's monitor.
- **notifyAll()

**: Wakes up all threads that are waiting on this object's monitor.

#### Thread Priorities
- Threads have priorities that determine how they should be scheduled.
- Use the setPriority() method to change the priority of a thread.
  ```java
  thread.setPriority(Thread.MAX_PRIORITY);
  ```

#### Deadlock, Starvation, and Thread Safety
- **Deadlock**: A situation where two or more threads are blocked forever, waiting for each other.
- **Starvation**: A situation where a thread is perpetually denied access to resources.
- **Thread Safety**: A thread-safe program ensures that no two threads can enter critical sections of code at the same time.

---

### **Day 22: Java 8 Features**

#### Lambda Expressions
- A new way of defining anonymous functions using a concise syntax.
  ```java
  (parameters) -> expression
  (parameters) -> { statements; }
  ```

#### Functional Interfaces
- An interface with exactly one abstract method, often used with lambda expressions.
  ```java
  @FunctionalInterface
  public interface MyFunctionalInterface {
      void myMethod();
  }
  ```

#### Streams API
- A new abstraction for working with sequences of elements in a functional style.
  ```java
  List<String> list = Arrays.asList("a", "b", "c");
  list.stream().filter(s -> s.startsWith("a")).forEach(System.out::println);
  ```

#### Optional Class
- A container object used to contain not-null objects and avoid null pointer exceptions.
  ```java
  Optional<String> optional = Optional.ofNullable(value);
  optional.ifPresent(System.out::println);
  ```

---

### **Day 23: Annotations**

#### Built-in Annotations
- **@Override**: Indicates that a method is overriding a method from the superclass.
- **@Deprecated**: Marks a method or class as deprecated.
- **@SuppressWarnings**: Instructs the compiler to suppress specific warnings.

#### Custom Annotations
- Creating your own annotations.
  ```java
  @Retention(RetentionPolicy.RUNTIME)
  @Target(ElementType.METHOD)
  public @interface MyAnnotation {
      String value();
  }
  ```

---

### **Day 24: Java 9 and Beyond**

#### Modules and the Module System
- A new way to group related packages and explicitly specify dependencies.
  ```java
  module my.module {
      requires java.base;
      exports com.example;
  }
  ```

#### JShell (Java Shell)
- A REPL (Read-Eval-Print Loop) tool for quickly testing Java code snippets.

#### Enhancements in Recent Java Versions
- New features and improvements in Java 9 through 17, such as:
  - **Local-Variable Type Inference** (`var` keyword)
  - **Text Blocks** for multi-line string literals
  - **Records** for immutable data classes
  - **Sealed Classes** for restricted class hierarchies

---

### **Day 25: Best Practices in Java**

#### Code Conventions
- Consistent naming, formatting, and code structure.
- Commenting and documentation practices.

#### Exception Handling Best Practices
- Proper use of try-catch blocks.
- Custom exception hierarchy.
- Logging exceptions.

#### Performance Optimization Tips
- Efficient use of data structures and algorithms.
- Avoiding unnecessary object creation.
- Lazy initialization and caching.

---

### **Day 26: Java Development Tools**

#### Build Tools
1. **Maven**: A build automation tool used primarily for Java projects.
   - POM (Project Object Model) file configuration.

2. **Gradle**: A flexible build automation tool.
   - Gradle scripts and configurations.

#### Version Control Systems
- **Git**: A distributed version control system for tracking changes in source code.
  - Basic commands: `git init`, `git clone`, `git add`, `git commit`, `git push`, `git pull`.

#### Debugging Techniques and Tools
- Debugging using IDE features (breakpoints, watches, step-through).
- Logging frameworks (SLF4J, Log4j).

---

### **Day 27: Design Patterns in Java**

#### Introduction to Design Patterns
- Best practices for solving common software design problems.

#### Singleton Pattern
- Ensures that a class has only one instance and provides a global point of access to it.

#### Factory Pattern
- A creational pattern that provides an interface for creating objects in a superclass but allows subclasses to alter the type of objects that will be created.

#### Observer Pattern
- A behavioral pattern where an object (subject) maintains a list of its dependents (observers) and notifies them of any state changes.

#### Strategy Pattern
- A behavioral pattern that enables selecting an algorithm's behavior at runtime.

---

### **Day 28: Java Testing**

#### Unit Testing with JUnit
- Writing and running unit tests to verify the behavior of individual components.

#### Test-Driven Development (TDD) Principles
- Writing tests before writing code.
- Refactoring code to improve design without changing behavior.

---

### **Day 29: Java Networking**

#### Basics of Networking in Java
- Networking concepts and protocols (TCP/IP, UDP).

#### Working with Sockets
- **ServerSocket** and **Socket** classes for server-client communication.

#### URL and HttpURLConnection Classes
- Working with URLs and HTTP requests.
  ```java
  URL url = new URL("http://example.com");
  HttpURLConnection conn = (HttpURLConnection) url.openConnection();
  ```

---

### **Day 30: Project and Review**

#### Building a Small Project
- Apply the concepts learned over the course to build a small Java project (e.g., a simple console application, a calculator, a basic CRUD application).

#### Reviewing Key Concepts
- Review all major topics covered, focusing on areas where you feel less confident.

#### Preparing for Further Learning
- Explore advanced Java topics like Java EE, Spring Framework, Hibernate, or delve into specialized areas like Android development or microservices.

---

This comprehensive guide should provide a solid foundation in Core Java over the next 30 days. Don't hesitate to reach out if you need further explanations or have specific questions as you go through each day's material!
