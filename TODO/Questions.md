
---
what if we have 2 methods in functional interface what will happen?


Widening Conversion in java \

spring gateway? 

stratergy design pattern


what is the best way to do the dependecy injection and why (constructor injection)

Discussed the message queues used and why we didn't use a standard message queue. 

Described the use case of Kafka in my application.

career aspirations 


code for producer and consumer problem in java

Shared a scenario where I had to debug issues with missing messages in Kafka.

how can we track in java what all endpoints have been hit and track them or log


https://itnext.io/understanding-oauth-2-0-architecture-use-cases-benefits-and-limitations-part-2-bad43ad4176 -- Auth Token


### **3. What is the MERGE Statement?** in sql

---

architecure of vymo
how to explain 
how we are doing the asynchronous programming 
how the containters are deployed
why sorting  is required 
array.sort() -> implementation
query for the max v

how I get ticket , how it gets assigned , how we working on it

---

marker interface
	
- Types of Garbage collector
    - Parallel
    - G1
    - Serial
    - Concurrent Mark Sweep

- Completable Future how to use it ?? Give examples
- - Dependency Injection ,Which one is least advisable ??
- - How does @Autowired access private singleton classes ?
- - How to resolve circular dependency in Spring ?
- - How to read yaml/properties file in Spring boot
    - `@Value`
    - `@ConfigurationProperties`
- Unit Testing
    - Difference between Spy and Mock
    - How to add Stub for void methods.
- - Microservices Design Pattern
    - SAGA
    - Database per service
- - HLD of File upload for large datasets.

- Implement a Caching Mechanism using 2 HashMaps, which will be accesed by multiple threads and delete data from cache if its timestamp crosses a TTL value


What is the difference between printing and logging
LRU cache, Course Schedule 2

sprind data JPA

What is CICD

 What is memory leak
Scaling in Microservice, which scenario which scaling is required
 Api gateway, circuit breaker 6. Data processing in kafka, consumer and producer
 AWS Services
 CI/CD pipeline Asked to draw a microservices architecture

What advantages does YAML offer over properties files in Spring Boot? Are there limitations when using YAML for configuration?

13. An easy design question. Design a service that will notify user on login/signup and credits them a point. Did this on [draw.io](http://draw.io/)
14. How I go on designing stuff keeping SOLID in mind

HLD for a food delivery app

 Big Integer multiplication, given number as String multiply them and store the result as string and return.
 Consider edge cases such as multiplication with "-0" etc.
 He asked about circuit breaker design pattern.
  CQRS design pattern,
  how would you improve the resiliency of a service,
  difference between map and flatmap
  java streams lazy if yes please explain how
  - Adapter pattern
- - SOLID Principles, particularly the Liskov substitution principle


class Test {
	public void m1(){
	   sop("no argument);
	}
	public void m1(int i) {
	  sop("int-argument");
	}
	public void m1(double d) {
	  sop("double-argument");
	}

     main() -->{
   Test t = new Test();
	t.m1();
	t.m1('a');



How to get the list of all the beans in your spring boot application?
Describe a Spring Boot project where you significantly improved performance. What techniques did you use?

Explain the concept of Spring Boot's embedded servlet containers.


How does Spring Boot make DI easier compared to traditionalSpring?

How does Spring Boot simplify the management of application
“secrets and sensitive configurations, especially when deployed
in different environments?

How can you enable and use asynchronous methods in a Spring
Boot application?
Describe how you would secure sensitive data in a Spring Boot
cPRiicalien that is accessed by multiple users with different
‘roles
You are creating an endpoint in a Spring Boot application that allows users to upload files. Explain how you would handle the file upload and where you would store the files.

‘What is Spring Boot CLI and how to execute the Spring Boot
‘project using boot CLI?

How Is Spring Security Implemented In A Spring Boot
Application?

How to Disable a Specific Auto-Configuration?

If you had to scale a Spring Boot application to handle high
‘traffic, what strategies would you use?

In Spring Boot, how is session management configured and handled, especially in distributed systems?

How does Spring Boot support internationalization (i18n)?

How do you mock microservices during testing?
Explain the process of creating a Docker image for a Spring ~ Boot application.

How can Spring Boot applications be made more resilient to failures,
~ especially in microservices architectures? |

finaally, finilized and final 

For audit purposes, your application requires a "soft delete" feature,
| where records are |Harked as deleted instead of being removed from the
| gidbase How would you implement this feature in your Spring Boot |
application:

 Once young space is full,?
- Experience in DDD, BDD, TDD
- Experience in backend testing using Junit/Mockito, MySQL, Kafka, and Avro.
- Familiarity with PCF apps, Docker, Kubernetes / Open shift
- - Strong experience in Micro services (Decompose, Strangler, Saga, Event sourcing, CQRS, Tx Messaging).
- autoboxing - boxing in generics
- 


4.Kafka basics and architecture
- About kafka
api endpoint security.
Cadinality  
ORM
Hashmap & hashset internal working
Creating Custom Set
String Pool
API's
- use of final key word?
- In a multithreaded environment how can I prevent re-assigning?

what are third party api's?? -- asked in a interview

why stored procedures are used, why used
thread local?
completable future
transaction propogations in java
aware interface
bean lifecycle
protype inject into singleton
microservices architecutre

2 beans dependent on each other how to solve this?

- ****Concurrency:**** How would you handle concurrent requests in a web application to ensure data consistency?
- ****Security:**** What measures would you take to secure a web application, especially regarding user authentication and data encryption?
- ****Scalability:**** How would you design a scalable system to handle a surge in user traffic, and what tools or services would you use?
- ****Error Handling:**** Describe your approach to implementing robust error handling in a backend service.


async annotation in java


amazon data lake 
JVM Tuning
Atomic Variables
Happens-Before Relationship
JWT, OAuth2, Authentication Providers
- Entity Lifecycle, Query Performance Optimization
- @EventListener, ApplicationEventPublisher
- Quartz, @Scheduled
- Resilience4j, Hystrix
REST, gRPC, WebSockets, Kafka
Bulkheading, Timeout Strategies
Saga Pattern, 2PC (Two-Phase Commit)
**Distributed Transactions** – Saga Pattern, 2PC (Two-Phase Commit)
CQRS & Event Sourcing
**Data Consistency in Microservices** – CAP Theorem, Idempotency
- **SQL Query Optimization** – Indexing, Query Execution Plan, Partitioning
- **ACID vs. BASE** – Eventual Consistency in NoSQL
- **MySQL Internals** – InnoDB vs. MyISAM, MVCC
- **PostgreSQL Deep Dive** – JSONB, CTEs, Window Functions
- **MongoDB** – Sharding, Replication, Aggregation Framework
- **Database Scaling Strategies** – Read/Write Splitting, Sharding, Federation
- **Kafka Internals** – Partitions, Consumer Groups, Offset Management
- - **Message Ordering & Exactly-Once Semantics**
- **Kafka vs. RabbitMQ vs. ActiveMQ**

15. **Event-Driven Architecture & Streaming Processing** – Kafka Streams, Flink


**Docker & Kubernetes** – K8s Networking, Stateful Sets, Helm

**CI/CD Pipelines** – Jenkins, GitHub Actions, ArgoCD

- **OWASP Top 10** – SQL Injection, XSS, CSRF, Clickjacking
- - **Custom Class Loaders & Dynamic Code Loading**
- - **JVM Locking Internals** – Biased Locking, Lock Elision
- **AOT Compilation in Java (GraalVM, SubstrateVM)**
eBPF for Java Performance Tuning


**Trade-Off Decisions** – When to Choose SQL vs. NoSQL, Monolith vs. Microservices


sage design
java 8 comparator
how to print odd even using mutlithreading
changes in java8 memory management

reflection in java

shallow copy & deep copy

why constructor name is same as class

why we need to to override hascode and equals when working iwth collections

volatile keyword

... dot operator in java

life cycle of a bean

sandboxing

git cherrypick

rebase

mvn clean and mvn install

if I have to scale high traffic application how to do that in springboot

grable collection algorithums'

softreference and weakreference in java

double brace initilization in java

how to implement caching in java

marker interface in java

what is functional programming 

how do memory leaks happen in java and how can we prevent it 

what is instance of variable'

java genrics

aggrigation composition association

autoboxing 

how will you customizae http response structure when a custom excetion occures , and how you handle mu

how will you handle different type of exceptions

how you handle for asynchronous methods 


which junit version4or5 or mockito version

what is code coverage, if I want too exclude a code how to do that 

so what happen if two pacages have the same class name

if your application frequenct gc pauses how would you optimize it.

tuning the heap size, 

callable and runnable difference

logging mechnaishm what we use in java ?? -- what is inbuild in springboot 


sealed classes

nullable keyword
thread deadlock

thread group

Spring AMQP
Spring Integration
- Spring Data;

ways to optimize the springboot application

serialversionuid

what is a immutable object in java , wnd why it is required 

how does immutablity provide thread safty? give with an example

could the constant creation of immutable object lead to garbage collection issues?

### 58. What do you understand by the jagged array?

how is deadloack occur in java'
### 51. How is the creation of a String using new() different from that of a literal?

what is a classloader

what is a string pool
16. What’s the difference between the methods sleep() and wait()?

### What are the different ways to create objects in Java?
### What are the advantages and disadvantages of object cloning?
### What is a marker interface?

aggrigation and composition

implementation of priorirty queue in java

### What is exception propagation?
### 163. What will happen if you put System.exit(0) on the try or catch block? Will finally block execute?
### What are the different types of Thread Priorities in Java? And what is the default priority of a thread assigned by JVM?

### 184. Explain the difference between a minor, major, and full garbage collection.
### 192. What are the JDBC API components?

### 194. What does the JDBC ResultSet interface?

### 195. What is the JDBC Rowset?

working of hasset in deep, in terms of interview

how can we make our own hashmap/hasset?

what is a parallel stream, under what conditon parallel stream will not provide performace benifit

in a data transformation pipeline, you need to process stream of stream of data -> flatmap -> advactage over simple map

compatable future -> how it is thread safetly

constructor chaning 

in jwt we have header, signature and other component so if we will change anything what will happen.

in microfservice there are mutiple and you need to authenticate once and allow same token on multiple services 

how do we store the secret key

what to do if we want to ensure no secret key can be pushed in the clould 

how was crudrepository different from springdatajpa

what is the difference between sending empty response entity instead of a full response entity

different port 

using different env


terminal operator
how to monitor different microservices? if one goes down

what are marker interface?
what is function interface?

immutable classes

spring bean lifecycle


1- Parent obj=new Child(); can obj be now called with an method of child class?
2 - a parent method throws IOException, but while overriding it in child we say it throws Exception, will it work?

transaction management in java

• Difference between linkedlist and arraylist which is faster to insert and delete.
• Size of long in java.
• Live use of BST.
• Can overload main function.
-  Given a String "Hello Epam, how are you ?", print the frequency of each word using streams only.
- - JVM, Heap memory, and Stack memory
- - Functional interfaces
- - Multi-threading and ExecutorService, threadpool
- - Adapter pattern
- 2 thread odd even print -- context switching odd even

Fibonacci series with memory optimisation, multi threading and lock concepts on code, questions on spring

write test case in java springboot

java memory allocation

what things I can do to make a application secure  java

@controller advice
@exceptionhandler

- Spring Security (JWT, OAuth2.0)
cllass ko mutable --

oberservable design pattern

nullable keyword

java stream using map

--------
misc 

what exactly is agile?

b. The candidate should be able to write unit test cases for
verifying the solution.
c. Candidate should be able to use Java 8+ versions.
d. Candidate should be able to write Java 8+ code for given
scenarios.
e. Candidate should know the concepts of selecting proper
Data Structures and Algorithm Techniques for Given
Problems.
f. Candidate should be able to complete each problem within
20 to 25 minutes.
g. There would be three problems, the candidate should solve.

TECHNICAL INTERVIEW – II
17. ID Verification: With clear visibility, the candidate should start the
video and present government-approved ID Proof to HR or
Interviewer.
18. The Interview Duration would be 90 Minutes after verification of ID
Proof.
19. During the 90 Minutes:
a. first two minutes, the interviewer introduces himself to the
candidate.
b. next five minutes the candidate introduces his achievement
and talks about his career.
c. After introductions, the next 60 to 70 minutes of technical
discussion.
d. The last 10 minutes of the interview duration will be
dedicated to the questions from the candidate.

20. Discussion and Coding:
a. Discussion on the current project, roles, and Responsibilities
b. Java Version 8+ Questions
i. JVM
ii. Multi-Threading
iii. Stream
iv. Lambda
v. Functional Interfaces
vi. Collections
vii. Date time APIs
viii. JVM memory model and architecture
c. Coding questions one or two
d. Should write Unit test cases.
i. Questions on various testing methods
e. Framework-related questions
i. Spring Framework
ii. REST API and So on.
f. SDLC – AGILE Related Questions

g. Estimation techniques
h. Design related Questions.
i. Architecture and Architecture Patterns
j. Mentoring, Learning and Lead related questions.



Serlizable ,

without transient keyword



21. Difference between Spring and Spring Boot  
22. How does a Spring Boot application determine the active profile?  
23. How to integrate multiple databases in a Spring Boot application?  
24. What is the difference between a Filter and an Interceptor?  
25. Explain the MVC workflow from frontend to backend.  
26. Authorization vs Authentication.  
27. How do you connect to a database in Spring Boot?  
28. Can we maintain sessions in REST APIS?  
29. What is Lombok?  
30. What is the Dispatcher Servlet?  
31. What are Spring Security and Spring Cloud?  
32. What is the IOC Container?  
33. What is Dependency Injection and its types? Which is recommended and why?  
34. What does @SpringBootApplication do?  
35. @Qualifier vs @Primary  
36. @RestController vs @Controller  
37. @RequestParam vs @PathVariable  
38. @Component vs @ComponentScan  
39. @ExceptionHandler vs @ControllerAdvice  
40. What is Spring Boot Actuator and how is it useful?  
41. What are the HTTP Methods you frequently use?



Confusing Questions 

* Covariant Return Type



Here’s a **deep-dive** list of **Core Java topics**, including advanced and rarely covered concepts:

---

### **1. Java Memory Management & Performance Tuning**

- **Heap & Stack Memory** – What goes where? Objects, References, Method Frames
- **Garbage Collection (GC) Algorithms** – Mark-Sweep, G1, ZGC, Shenandoah
- **JVM Tuning & Performance Optimization** – `-Xms`, `-Xmx`, `-XX:+UseG1GC`, `-XX:+PrintGCDetails`
- **Escape Analysis & Stack Allocation** – How JVM optimizes object creation
- **JIT Compilation & Code Optimization** – C1 (Client), C2 (Server), Graal JIT
- **Memory Barriers & Volatile** – Happens-Before relationship
- **Reference Types & Their Impact on GC** – Soft, Weak, Phantom References
- **String Pool & Interning** – How `String.intern()` saves memory

---

### **2. Java Class Loading Mechanism**

- **Bootstrap, Extension & Application ClassLoaders**
- **Custom Class Loaders** – Creating your own `ClassLoader`
- **Dynamic Class Loading & Reflection** – `Class.forName()`, `Method.invoke()`
- **JVM Class Verification Process** – Bytecode verification steps
- **Java Instrumentation API** – Modifying bytecode at runtime

---

### **3. Multithreading & Concurrency (Deep Concepts)**

- **Thread Lifecycle & State Transitions**
- **Thread Coordination Mechanisms** – `wait()`, `notify()`, `notifyAll()`
- **Java Memory Model (JMM)** – Happens-Before, Visibility, Reordering
- **CAS (Compare-And-Swap) & Atomic Operations** – `AtomicInteger`, `Unsafe`
- **ReentrantLock vs. Synchronized** – Fair Locking, Starvation, Biasing
- **ThreadLocal & InheritableThreadLocal** – Managing thread-specific data
- **ForkJoinPool vs. ExecutorService** – Work-stealing algorithm

---

### **4. Java Collections (Deep Dive)**

- **HashMap Internal Working** – Hashing, Collision Handling, Treeification
- **Concurrent Collections** – `ConcurrentHashMap`, `CopyOnWriteArrayList`
- **Why HashMap key should be immutable?**
- **BlockingQueues & Producer-Consumer Pattern** – `LinkedBlockingQueue`, `ArrayBlockingQueue`
- **PriorityQueue & Its Implementation** – Binary Heap structure
- **WeakHashMap, IdentityHashMap, EnumMap** – Specialized maps in Java

---

### **5. Serialization & Deserialization (Advanced)**

- **Serializable vs. Externalizable** – Performance implications
- **Serial Version UID & Object Stream Protocol**
- **Deep Cloning using Serialization**
- **Custom Serialization with `writeObject()` and `readObject()`**
- **Preventing Serialization Attacks** – `readResolve()` and `writeReplace()`
- **Kryo & JSON-Based Serialization Alternatives**

---

### **6. Reflection API & Dynamic Proxies**

- **Creating Objects at Runtime using Reflection** – `Constructor.newInstance()`
- **Accessing Private Fields & Methods** – `setAccessible(true)`
- **Method Handles & Invokedynamic (Java 7+)**
- **Bytecode Manipulation Libraries** – ASM, Javassist, ByteBuddy
- **Creating Dynamic Proxies** – `Proxy.newProxyInstance()`

---

### **7. Functional Programming & Java Streams**

- **Lambda Internals & Synthetic Methods**
- **Lazy Evaluation in Streams** – How Streams process elements
- **Short-Circuiting Operations** – `limit()`, `findFirst()`, `anyMatch()`
- **Custom Collectors & Reduction Strategies** – `Collectors.toMap()`, `Collectors.groupingBy()`
- **Parallel Streams & ForkJoinPool** – When to use, when not to use

---

### **8. Exception Handling & Best Practices**

- **Checked vs. Unchecked Exceptions** – When to use which
- **Suppressed Exceptions in Try-With-Resources**
- **Custom Exception Handling Strategies**
- **Best Practices for Logging Exceptions** – Structured logging, SLF4J, Logback

---

### **9. Java Modules (JPMS - Java 9)**

- **Modularization in Java** – `module-info.java`
- **Automatic Modules & Migration Strategies**
- **Reflection Restrictions & Encapsulation in Modules**

---

### **10. Advanced String Handling & Optimization**

- **How `StringBuilder` Works Internally**
- **String Deduplication in G1 GC**
- **Substring Memory Leak in Older Java Versions**

---

### **11. Compiler & Optimization Techniques**

- **Escape Analysis & Scalar Replacement**
- **Inlining & Devirtualization in JIT Compiler**
- **Loop Unrolling & Auto-Vectorization**

---

### **12. Java Agent Programming**

- **JVM Instrumentation API** – Attaching Agents Dynamically
- **Code Injection using Java Agents**
- **Profiling & Monitoring Using Agents**

---

### **13. Metaspace & Native Memory Usage**

- **Metaspace vs. PermGen (Java 8+ Changes)**
- **Class Metadata Storage & Impact on GC**
- **Native Memory Tracking (NMT) in Java**

---

### **14. Java Security & Cryptography**

- **Java Security Manager (Deprecated in Java 17)**
- **KeyStore & SecureRandom API**
- **TLS/SSL & Cipher Suites in Java**
- **Password Hashing & PBKDF2, BCrypt, Argon2**

---

### **15. Low-Level JVM Topics**

- **Biased Locking & Lock Elision**
- **Escape Analysis & Allocation Elimination**
- **Java Unsafe API** – Direct Memory Access
- **GraalVM & Ahead-of-Time (AOT) Compilation**

---

### **Rarely Covered Topics**

- **Zero-Cost Abstractions in Java** – Optimizing Runtime Performance
- **eBPF for Java Performance Tuning** – Deep Kernel-Level Observability
- **How `synchronized` Works Internally** – Object Header & Lock Word
- **Why `volatile` is Not Enough for Atomicity** – Happens-Before & Visibility Guarantees
- **Profiling Tools for Java** – JFR, async-profiler, perf, bpftrace



---

microservice design patterns -- need 

caching states


Distributed Transactions 


---
1) what are static blocks and static initalizers in Java ?.......................................................... 9 2) How to call one constructor from the other constructor ? ............................................... 9 3) What is method overriding in java ? ........................................................................................ 9 4) What is super keyword in java ? ................................................................................................. 9 5) Difference between method overloading and method overriding in java ?............... 9 6) Difference between abstract class and interface ?............................................................ 10 7) Why java is platform independent?................................................................................... 10 8) What is method overloading in java ?.............................................................................. 10 9) What is difference between c++ and Java ? ................................................................. 10 10) What is JIT compiler ?.............................................................................................................. 10 11) What is bytecode in java ? ................................................................................................. 10 12) Difference between this() and super() in java ? ...................................................... 11 13) What is a class ? .................................................................................................................... 11 14) What is an object ?.................................................................................................................... 11 15)What is method in java ? ............................................................................................................ 11 16) What is encapsulation ? ............................................................................................................ 11 17) Why main() method is public, static and void in java ? ............................................... 12 18) Explain about main() method in java ? .............................................................................. 12 19)What is constructor in java ?..................................................................................................... 12 20) What is difference between length and length() method in java ?......................... 12 21) What is ASCII Code?........................................................................................................... 12 22) What is Unicode ? .................................................................................................................. 13 23) Difference between Character Constant and String Constant in java ?............ 13 24) What are constants and how to create constants in java? ........................................ 13 25) Difference between ‘>>’ and ‘>>>’ operators in java?.............................................. 13 Core java Interview questions on Coding Standards .................................................................. 13 26) Explain Java Coding Standards for classes or Java coding conventions for classes?..................................................................................................................................................... 13 27) Explain Java Coding standards for interfaces? ........................................................... 13 2 28) Explain Java Coding standards for Methods?.............................................................. 13 29) Explain Java Coding Standards for variables ?............................................................... 13 30) Explain Java Coding Standards for Constants? .............................................................. 13 31) Difference between overriding and overloading in java? ....................................... 14 32) What is ‘IS-A ‘ relationship in java? .............................................................................. 14 33) What is ‘HAS A’’ relationship in java?............................................................................... 14 34) Difference between ‘IS-A’ and ‘HAS-A’ relationship in java? .................................... 14 35) Explain about instanceof operator in java? ....................................................................... 14 36) What does null mean in java? ................................................................................................ 15 37) Can we have multiple classes in single file ? ..................................................................... 15 38) What all access modifiers are allowed for top class ? ................................................... 15 39 ) What are packages in java? .................................................................................................... 15 40) Can we have more than one package statement in source file ?........................ 15 41) Can we define package statement after import statement in java? ...................... 15 42) What are identifiers in java?............................................................................................... 15 43) What are access modifiers in java? ................................................................................... 15 44) What is the difference between access specifiers and access modifiers in java?16 45) What access modifiers can be used for class ?..................................................... 16 46) Explain what access modifiers can be used for methods?........................................ 16 47) Explain what access modifiers can be used for variables? ....................................... 16 48) What is final access modifier in java? ...................................................................... 17 49) Explain about abstract classes in java? ................................................................... 17 50) Can we create constructor in abstract class ?....................................................... 18 51) What are abstract methods in java? ................................................................................. 18 Java Exception Handling Interview questions................................................................................ 18 52) What is an exception in java?.............................................................................................. 18 53) State some situations where exceptions may arise in java? ................................... 18 54) What is Exception handling in java? ......................................................................... 18 55) What is an eror in Java?................................................................................................ 18 56) What are advantages of Exception handling in java?................................................. 18 57) In how many ways we can do exception handling in java? ..................................... 18 58) List out five keywords related to Exception handling ?.............................................. 18 3 59) Explain try and catch keywords in java?................................................................. 19 60) Can we have try block without catch block?.......................................................... 19 61) Can we have multiple catch block for a try block? ...................................................... 19 62) Explain importance of finally block in java? ................................................................... 19 63) Can we have any code between try and catch blocks?.................................................. 19 64) Can we have any code between try and finally blocks? .................................... 19 65) Can we catch more than one exception in single catch block?.................................. 19 66) What are checked Exceptions?............................................................................................ 20 67) What are unchecked exceptions in java? ........................................................................ 20 68) Explain differences between checked and Unchecked exceptions in java?........ 20 69) What is default Exception handling in java? .......................................................... 20 70) Explain throw keyword in java?.................................................................................. 21 71) Can we write any code after throw statement?............................................................ 21 72) Explain importance of throws keyword in java? ........................................................... 21 73) Explain the importance of finally over return statement? ........................................ 21 74) Explain a situation where finally block will not be executed? ......................... 21 75) Can we use catch statement for checked exceptions? ...................................... 21 76) What are user defined exceptions?.................................................................................... 21 77) Can we rethrow the same exception from catch handler?...................................... 21 78) Can we nested try statements in java?................................................................................ 22 79) Explain the importance of throwable class and its methods? ......................... 22 80) Explain when ClassNotFoundException will be raised ? .............................................. 22 81) Explain when NoClassDefFoundError will be raised ? .................................................. 22 Java Interview questions on threads................................................................................................. 22 83) What is process ?...................................................................................................................... 22 84) What is thread in java? .......................................................................................................... 22 85) Difference between process and thread? ........................................................................ 22 86) What is multitasking ? ............................................................................................................ 22 87) What are different types of multitasking?....................................................................... 22 88) What are the benefits of multithreaded programming? ........................................... 23 89) Explain thread in java?........................................................................................................... 23 90) List Java API that supports threads?................................................................................. 23 4 91) Explain about main thread in java? ....................................................................................... 23 92) In how many ways we can create threads in java? ....................................................... 23 93) Explain creating threads by implementing Runnable class? .................................... 23 94) Explain creating threads by extending Thread class ? ............................................... 23 95) Which is the best approach for creating thread ? ........................................................ 24 96) Explain the importance of thread scheduler in java?................................................... 24 97) Explain the life cycle of thread?.......................................................................................... 24 98) Can we restart a dead thread in java? ............................................................................. 24 99) Can one thread block the other thread?.......................................................................... 24 100) Can we restart a thread already started in java?..................................................... 24 101) What happens if we don’t override run method ? ........................................................ 24 102) Can we overload run() method in java?........................................................................ 24 105) What is a lock or purpose of locks in java?.................................................................. 24 106) In how many ways we can do synchronization in java? ......................................... 25 107) What are synchronized methods ? .................................................................................. 25 108) When do we use synchronized methods in java?......................................................... 25 109) When a thread is executing synchronized methods , then is it possible to execute other synchronized methods simultaneously by other threads? ...................... 25 110) When a thread is executing a synchronized method , then is it possible for the same thread to access other synchronized methods of an object ?.................................. 25 111) What are synchronized blocks in java?.............................................................................. 25 112) When do we use synchronized blocks and advantages of using synchronized blocks? ...................................................................................................................................................... 25 113) What is class level lock ?......................................................................................................... 26 114) Can we synchronize static methods in java? ................................................................. 26 115) Can we use synchronized block for primitives?............................................................. 26 116) What are thread priorities and importance of thread priorities in java? ............. 26 117) Explain different types of thread priorities ? ............................................................... 26 118) How to change the priority of thread or how to set priority of thread?............... 26 119) If two threads have same priority which thread will be executed first ?............. 26 120) What all methods are used to prevent thread execution ? ..................................... 26 121) Explain yield() method in thread class ?........................................................................... 26 122) Is it possible for yielded thread to get chance for its execution again ? ............. 27 5 123) Explain the importance of join() method in thread class? ..................................... 27 124) Explain purpose of sleep() method in java?................................................................... 27 125) Assume a thread has lock on it, calling sleep() method on that thread will release the lock? ................................................................................................................................... 28 126) Can sleep() method causes another thread to sleep? ............................................. 28 127) Explain about interrupt() method of thread class ?.................................................. 28 128) Explain about interthread communication and how it takes place in java? ....... 28 129) Explain wait(), notify() and notifyAll() methods of object class ? ......................... 28 130) Explain why wait() , notify() and notifyAll() methods are in Object class rather than in thread class? ........................................................................................................................... 28 131) Explain IllegalMonitorStateException and when it will be thrown? ......................... 28 132) when wait(), notify(), notifyAll() methods are called does it releases the lock or holds the acquired lock? ............................................................................................................... 28 133) Explain which of the following methods releases the lock when yield(), join(),sleep(),wait(),notify(), notifyAll() methods are executed? ...................................... 28 134) What are thread groups? ....................................................................................................... 29 135) What are thread local variables ? ........................................................................................ 29 136) What are daemon threads in java? ..................................................................................... 29 137) How to make a non daemon thread as daemon? .......................................................... 29 138) Can we make main() thread as daemon? ....................................................................... 29 Interview questions on Nested classses and inner classes....................................................... 29 139) What are nested classes in java? ....................................................................................... 29 140) What are inner classes or non static nested classes in java? ................................... 29 141) Why to use nested classes in java? ................................................................................... 29 (or) ............................................................................................................................................................. 29 What is the purpose of nested class in java?............................................................................. 29 142) Explain about static nested classes in java? .................................................................. 30 143) How to instantiate static nested classes in java? .......................................................... 30 144) Explain about method local inner classes or local inner classes in java?............ 30 145) Explain about features of local inner class? ..................................................................... 30 146) Explain about anonymous inner classes in java?........................................................... 30 147) Explain restrictions for using anonymous inner classes?............................................ 30 148) Is this valid in java ? can we instantiate interface in java?...................................... 30 6 149) Explain about member inner classes?................................................................................ 30 150) How to instantiate member inner class? ........................................................................... 31 151) How to do encapsulation in Java?........................................................................................ 31 152) What are reference variables in java? .............................................................................. 31 153) Will the compiler creates a default constructor if I have a parameterized constructor in the class? .................................................................................................................... 31 154) Can we have a method name same as class name in java?.................................... 31 155) Can we override constructors in java? ............................................................................. 31 156) Can Static methods access instance variables in java?............................................... 31 157) How do we access static members in java?..................................................................... 31 158) Can we override static methods in java? ....................................................................... 31 159) Difference between object and reference?....................................................................... 31 160 ) Objects or references which of them gets garbage collected?................................ 32 161) How many times finalize method will be invoked ? who invokes finalize() method in java?..................................................................................................................................... 32 162) Can we able to pass objects as an arguments in java?............................................... 32 163) Explain wrapper classes in java?.......................................................................................... 32 164) Explain different types of wrapper classes in java? ...................................................... 32 165) Explain about transient variables in java?........................................................................ 32 166) Can we serialize static variables in java?.......................................................................... 32 167) What is type conversion in java?........................................................................................ 32 168) Explain about Automatic type conversion in java? ...................................................... 32 169) Explain about narrowing conversion in java?.................................................................. 33 170) Explain the importance of import keyword in java? ..................................................... 33 171) Explain naming conventions for packages ? .................................................................... 33 172) What is classpath ?.................................................................................................................... 33 173) What is jar ?................................................................................................................................. 33 174) What is the scope or life time of instance variables ?.................................................. 33 175) Explain the scope or life time of class variables or static variables?...................... 33 176) Explain scope or life time of local variables in java? .................................................... 33 177) Explain about static imports in java? ................................................................................ 33 178) Can we define static methods inside interface? ............................................................. 34 7 179) Define interface in java?.......................................................................................................... 34 180) What is the purpose of interface?........................................................................................ 34 181) Explain features of interfaces in java? ............................................................................... 34 182) Explain enumeration in java? ................................................................................................ 34 183) Explain restrictions on using enum?.................................................................................. 34 184) Explain about field hiding in java?....................................................................................... 34 185) Explain about Varargs in java?............................................................................................ 34 186) Explain where variables are created in memory?.......................................................... 35 187) Can we use Switch statement with Strings?.................................................................... 35 188) In java how do we copy objects?......................................................................................... 35 Oops concepts interview questions.................................................................................................... 35 189) Explain about procedural programming language or structured programming language and its features?............................................................................................................... 35 190) Explain about object oriented programming and its features?................................. 35 191) List out benefits of object oriented programming language?.................................... 35 192) Differences between traditional programming language and object oriented programming language? .................................................................................................................... 35 193) Explain oops concepts in detail? ......................................................................................... 35 194) Explain what is encapsulation? ............................................................................................. 36 195) What is inheritance ?............................................................................................................... 36 196) Explain importance of inheritance in java?..................................................................... 36 197) What is polymorphism in java?............................................................................................. 36 Collection Framework interview questions...................................................................................... 36 198) What is collections framework ?........................................................................................... 36 199) What is collection ?.................................................................................................................... 37 200) Difference between collection, Collection and Collections in java?......................... 37 201) Explain about Collection interface in java ?.................................................................... 37 202) List the interfaces which extends collection interface ? ............................................. 37 203) Explain List interface ? ............................................................................................................. 37 204) Explain methods specific to List interface ? ..................................................................... 38 205) List implementations of List Interface ? ............................................................................ 38 206) Explain about ArrayList ? ....................................................................................................... 38 8 207) Difference between Array and ArrayList ? ........................................................................ 38 208) What is vector?.......................................................................................................................... 39 209) Difference between arraylist and vector ?........................................................................ 39 210) Define Linked List and its features with signature ? .................................................. 39 211) Define Iterator and methods in Iterator? ........................................................................ 40 212) In which order the Iterator iterates over collection?.................................................... 40 212) Explain ListIterator and methods in ListIterator?......................................................... 40 213) Explain about Sets ? ................................................................................................................. 41 214) Implementations of Set interface ?..................................................................................... 41 215) Explain HashSet and its features ? .................................................................................... 41 216) Explain Tree Set and its features?....................................................................................... 41 217) When do we use HashSet over TreeSet? .......................................................................... 42 218) What is Linked HashSet and its features? ........................................................................ 42 219) Explain about Map interface in java?.................................................................................. 42 220) What is linked hashmap and its features?........................................................................ 42 221) What is SortedMap interface? .............................................................................................. 42 222) What is Hashtable and explain features of Hashtable? .............................................. 42 223) Difference between HashMap and Hashtable? ................................................................ 42 224) Difference between arraylist and linkedlist? .................................................................... 43 225) Difference between Comparator and Comparable in java? ...................................... 43 226) What is concurrent hashmap and its features ?............................................................. 43 227) Difference between Concurrent HashMap and Hashtable and collections.synchronizedHashMap? ................................................................................................ 43 228) Explain copyOnWriteArrayList and when do we use copyOnWriteArrayList? ...... 43 229) Explain about fail fast iterators in java?............................................................................ 44 230) Explain about fail safe iterators in java?........................................................................... 44 Core java Serialization interview questions .................................................................................... 44 231) What is serialization in java? ................................................................................................. 44 232) What is the main purpose of serialization in java?........................................................ 44 233) What are alternatives to java serialization?..................................................................... 44 234) Explain about serializable interface in java?.................................................................... 44 235) How to make object serializable in java?.......................................................................... 44 9 236) What is serial version UID and its importance in java?............................................... 44 237) What happens if we don’t define serial version UID ? ................................................. 45 238) Can we serialize static variables in java?.......................................................................... 45 239) When we serialize an object does the serialization mechanism saves its references too? ...................................................................................................................................... 45 240) If we don’t want some of the fields not to serialize How to do that?..................... 45

