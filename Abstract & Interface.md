
---

## **1. Abstract Class**

### **Variables in an Abstract Class**

1. **Types of Variables**:
    
    - Can include **instance variables**, **static variables**, and **final variables**.
    - These variables can have any access modifier (`public`, `private`, `protected`).
2. **Initialization**:
    
    - Variables can be initialized directly or in the constructor of the abstract class.
3. **Behavior**:
    
    - They follow standard object-oriented principles.
    - Instance variables belong to the object, while static variables belong to the class.

---

### **Functions in an Abstract Class**

1. **Abstract Methods**:
    
    - Defined with the `abstract` keyword.
    - Do not have a body (implementation).
    - Must be implemented in the first concrete subclass.
    
    ```java
    abstract void displayMessage();
    ```
    
2. **Concrete Methods**:
    
    - Abstract classes can also have methods with full implementation.
    - These can be inherited by subclasses or overridden.
    
    ```java
    void show() {
        System.out.println("This is a concrete method in the abstract class.");
    }
    ```
    
3. **Access Modifiers**:
    
    - Methods can have any access modifier: `public`, `protected`, or `private`.
4. **Static and Final Methods**:
    
    - Abstract classes can have `static` and `final` methods.
    - `static` methods belong to the class and cannot be overridden.
    - `final` methods cannot be overridden in subclasses.

---

### **Example of an Abstract Class**

```java
abstract class Shape {
    private String color; // Instance variable
    static int count; // Static variable

    // Constructor
    public Shape(String color) {
        this.color = color;
    }

    // Abstract method
    abstract void draw();

    // Concrete method
    public void displayColor() {
        System.out.println("Color: " + color);
    }
}
```

---

## **2. Interface**

### **Variables in an Interface**

1. **Nature**:
    
    - Variables in an interface are implicitly:
        - `public`
        - `static`
        - `final`
    - This means they are **constants** and cannot be changed once defined.
2. **Initialization**:
    
    - Must be initialized at the time of declaration.
3. **Behavior**:
    
    - Variables belong to the interface itself, not the implementing class.
    
    ```java
    interface Test {
        int MAX_LIMIT = 100; // Implicitly public static final
    }
    ```
    

---

### **Functions in an Interface**

1. **Abstract Methods**:
    
    - Before Java 8, interfaces could only have abstract methods.
    - These are implicitly `public` and `abstract`.
    
    ```java
    void displayMessage(); // Implicitly public abstract
    ```
    
2. **Default Methods (Java 8)**:
    
    - Introduced in Java 8.
    - Methods with implementation.
    - Can be overridden by implementing classes.
    
    ```java
    default void show() {
        System.out.println("Default method in an interface.");
    }
    ```
    
3. **Static Methods (Java 8)**:
    
    - Methods that belong to the interface, not the implementing class.
    - Cannot be overridden.
    
    ```java
    static void log(String message) {
        System.out.println("Log: " + message);
    }
    ```
    
4. **Private Methods (Java 9)**:
    
    - Helper methods used within the interface.
    - Cannot be accessed by implementing classes.
    
    ```java
    private void helper() {
        System.out.println("Private method in an interface.");
    }
    ```
    

---

### **Example of an Interface**

```java
interface Animal {
    int MAX_AGE = 100; // public static final

    // Abstract method
    void sound();

    // Default method
    default void eat() {
        System.out.println("This animal is eating.");
    }

    // Static method
    static void info() {
        System.out.println("This is an Animal interface.");
    }
}
```

---

## **Key Differences**

| Feature            | Abstract Class                                               | Interface                                                |
| ------------------ | ------------------------------------------------------------ | -------------------------------------------------------- |
| **Variables**      | Can be `private`, `protected`, or `public`.                  | Always `public static final` (constants).                |
| **Initialization** | Variables can be initialized directly or in the constructor. | Must be initialized at the time of declaration.          |
| **Methods**        | Can have abstract, concrete, static, or final methods.       | Can have abstract, default, static, and private methods. |
| **Inheritance**    | A class can inherit only one abstract class.                 | A class can implement multiple interfaces.               |
| **Constructors**   | Can have constructors.                                       | Cannot have constructors.                                |

---
