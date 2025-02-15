
---

SOLID principles are a set of design guidelines that help make software systems more maintainable, flexible, and scalable.

## **1. Single Responsibility Principle (SRP)**

### **Rule:**

A class should have only **one reason to change**.

### **Meaning:**

Every class should have a **single job** or responsibility.

### **Example:**

**Bad Design:**

```java
class Book {
    String title;
    String author;
    
    public void print() {
        System.out.println("Title: " + title + "\nAuthor: " + author);
    }
}
```

**Good Design:**

```java
class Book {
    String title;
    String author;
}

class Printer {
    public void print(Book book) {
        System.out.println("Title: " + book.title + "\nAuthor: " + book.author);
    }
}
```

---
## **2. Open/Closed Principle (OCP)**

### **Rule:**

A class should be **open for extension but closed for modification**.

### **Meaning:**

New features should be added **without modifying existing code**.

### **Example:**

**Good Design:**

```java
abstract class Shape {
    abstract void draw();
}

class Circle extends Shape {
    void draw() {
        System.out.println("Drawing Circle");
    }
}

class Rectangle extends Shape {
    void draw() {
        System.out.println("Drawing Rectangle");
    }
}

class Triangle extends Shape {
    void draw() {
        System.out.println("Drawing Triangle");
    }
}
```

---
## **3. Liskov Substitution Principle (LSP)**

### **Rule:**

A subclass should be **replaceable** for its parent class **without breaking the program**.

### **Meaning:**

If `B` is a subclass of `A`, then `B` should be usable **wherever** `A` is expected **without errors**.

### **Example:**

**Bad Design:**

```java
class Bird {
    void fly() {
        System.out.println("Bird is flying");
    }
}

class Penguin extends Bird {
    void fly() {
        throw new UnsupportedOperationException("Penguins can't fly!");
    }
}
```

**Good Design:**

```java
class Bird {
    String name;
}

class FlyingBird extends Bird {
    void fly() {
        System.out.println(name + " is flying");
    }
}

class Penguin extends Bird {
    void swim() {
        System.out.println(name + " is swimming");
    }
}
```

---
## **4. Interface Segregation Principle (ISP)**

### **Rule:**

Do not force a class to implement interfaces it **doesn’t use**.

### **Meaning:**

Split large interfaces into **smaller, specific** ones.

### **Example:**

**Bad Design:**

```java
interface Robot {
    void fly();
    void swim();
}

class HumanoidRobot implements Robot {
    public void fly() {
        System.out.println("Flying in the sky");
    }
    
    public void swim() {
        System.out.println("Swimming in water");
    }
}
```

**Good Design:**

```java
interface Flyable {
    void fly();
}

interface Swimmable {
    void swim();
}

class Bird implements Flyable {
    public void fly() {
        System.out.println("Bird is flying");
    }
}

class Fish implements Swimmable {
    public void swim() {
        System.out.println("Fish is swimming");
    }
}
```

---
## **5. Dependency Inversion Principle (DIP)**

### **Rule:**

Depend on **abstractions (interfaces)**, not on **concrete implementations**.

### **Meaning:**

High-level modules should not depend **directly** on low-level modules.

### **Example:**

**Bad Design:**

```java
class PaymentService {
    private CreditCard creditCard;
    
    public PaymentService() {
        this.creditCard = new CreditCard();
    }
    
    public void processPayment() {
        creditCard.pay();
    }
}
```

**Good Design:**

```java
interface PaymentMethod {
    void pay();
}

class CreditCard implements PaymentMethod {
    public void pay() {
        System.out.println("Payment using Credit Card");
    }
}

class PayPal implements PaymentMethod {
    public void pay() {
        System.out.println("Payment using PayPal");
    }
}

class PaymentService {
    private PaymentMethod paymentMethod;
    
    public PaymentService(PaymentMethod paymentMethod) {
        this.paymentMethod = paymentMethod;
    }
    
    public void processPayment() {
        paymentMethod.pay();
    }
}
```

---

## **💡 Summary of SOLID Principles**

|**Principle**|**Rule**|
|---|---|
|**S**ingle Responsibility|A class should have **one job**.|
|**O**pen/Closed|Code should be **open for extension**, **closed for modification**.|
|**L**iskov Substitution|Subclasses should be **replaceable** without breaking code.|
|**I**nterface Segregation|Interfaces should be **small and specific**.|
|**D**ependency Inversion|Depend on **abstractions**, not **concrete implementations**.|
