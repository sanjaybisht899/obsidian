
**Kafka:**

- Explained the architecture.
- Discussed the message queues used and why we didn't use a standard message queue.
- Described the use case of Kafka in my application.
- Shared a scenario where I had to debug issues with missing messages in Kafka.

**Java:**

- Discussed the version of Java I am using.
- Talked about streams and filters.
- Mentioned the features of Java 11 I have used.
- Explained the use of data structures like binary trees for code optimization.
- Described my experience with multithreading and the thread lifecycle.

**Authorization Module:**

- Explained the working of the authorization module, token generation, and validation.

**Camunda Workflows:**

- Described how Camunda workflows function and interact with the code.

**Performance Optimizations:**

- Discussed any performance optimizations I have made in the application.
- CICD Framework and Cloud Usage:
    - Briefly talked about my work in the CICD framework and the cloud used (no in-depth questions).
---
**Round 1:**

- What is the difference between TCP and UDP?
- What is Secure Socket Layer (SSL)?
- Full current project discussion in deep.
- [Symmetric Tree](https://leetcode.com/problems/symmetric-tree/)

---
Round 2 -> Taken by Principle engineer  
Ask is to Give low level design of Cache with both LRU AND LFU as Eviction algorithim .  
This round streached till 1.5 hrs , discussed code and various design stratergies to implement .

---

**Round 2 Technical Interview**  
I was asked to explain the approach and why for both the problems and was given a slight modification in test cases in one of the problems but I don't remember it actually now. After that I was asked this problem :  
_There are two data sets consisting of random numbers from 1 to 50K in one array and 1 to 60K in another array. I have with me only an array of size 10 and I have to sort both the arrays 50K + 60K resulting in an array os 110K elements which are to be sorted in ascending order._  
I told them that I can use a sliding window to try and sort the elements, but I did not know how to implement it nor did i know if the approach was right. I however explained to him that I can sort the 50K and 60K arrays in-place using quicksort and can combine them using the logic of mergesort. I explained both of the sorting algos to the interview. He told it's okay if I didn't know the solution to this and we moved on.  
Next he asked a couple of questions on sql , used a sample Employee table and asked questions using joins, subqueries and filter using where clause. A problem where I should GroupBy using primary key.

---

F2F Interview 1 (Technical)(45 min):

Due to large number of candidates shortlisted for interviews, each interviewer was handling 2-3

candidates simultaneously . He directly fired different coding questions on us without wasting even a

second. I was given to implement next_permutation() function of c++ and the other student was

asked about the excel sheet problem [http://www.geeksforgeeks.org/find-excel-column-name-givennumber/](http://www.geeksforgeeks.org/find-excel-column-name-givennumber/).

After this round I was told to wait outside. Another interviewer was present there and he quickly

asked me 2 more coding questions [http://www.geeksforgeeks.org/a-product-array-puzzle/](http://www.geeksforgeeks.org/a-product-array-puzzle/) and the

other question was - given a paragraph find which alphabet doesn’t occur in it. The key to this round

was to give simple, quick and optimal solution wrt time and space. A normal solution led to direct

exit from this round without any deliberations.

---
### **Round 2: Technical (Project & DSA)**

- **Project-related questions** (architecture, challenges, decision-making)
- Some **managerial** questions
- **1 Hard DSA problem** (solved in 45 mins with hints)
- Call extended for **30 mins** for:
    - **SQL queries**
    - **Java Streams API** questions
---
**1st Round**

1. Introduction and cross-questioning on design aspects of previous projects
2. Given an array of integers and an integer k  
    You can perform the below operation at most k times. Find maximum possible OR value of the array (Bitwise OR of all elements in the array).
    1. Choose any index in the array
    2. Multiply the number at that index by 2

---

Round 1 - System Design  
Design Stock Exchange

---
Round 1(LLD):  
Behavioral questions.  
Provide LLD for Task scheduler.

---
### Round 1(On-site)

My on-site interview was divided into two parts. The first part focused on Java Core, Data Structures and Algorithms (DSA), Math Puzzles, and previous work experience. The second part was entirely dedicated to Database Management and SQL queries. The questions included:

**Java Core:**

- How does immutability works in java?
- How to create an immutable class?
- Can a class be static? If yes, then where it can be used?
- Difference in C++ and Java.
- How does string addition work in Java?(s1 = s1+s2)
- In which case does the finally block does not execute?

**DSA:**

- Get the Longest Valid Parentheses sequence.  
    Example: For the string "((())()()", the answer would be 8, which corresponds to "(())()()".

**Math Puzzles:**

- Last Palindrome Date (gfg puzzle)
- Three boxes have two balls inside. One with two green, one with two red and one with 1 red & 1 green. All the boxes are labelled as GG, RR and RG. What if I change all the labels to be incorrect, like GG labelled box will never have 2 green ball, it would either have 2 red balls or 1 green and 1 red ball. Now we have to take out one ball from any of the box of our choice and have to tell what are the right label for all of the boxes.
- Door Puzzle (Classic puzzle on gfg)

**DB and SQL:**

- There were some questions on Hibernate on how it works?
- Queries on Cartesian Product, Full Join, left Join.
- Lazy Loading in Spring Boot
- @Transaction Management in Hibernate.
- Some questions on Indexing.
- Primary Key vs Unique Key
- Having vs Where clause
- Normalization upto 3NF
- Read and Write locking in DB.

---

```
Round1 (Problem Solving)
1. Minimum Add to Make Parentheses Valid. https://leetcode.com/problems/minimum-add-to-make-parentheses-valid/
2. Minimum appends required to make a string palindrome.
3. Longest sub-array having sum K.
```

---

**Interview Round 1**  
This round was taken by a Senior Application Developer of oracle SCM Cloud. He asked me about my experience and in which tech stack I am currently working. Then he gave me a dsa question.

Q1 : Given an integer array nums, find the contiguous subarray (containing at least one number) which has the largest sum and return its sum. A subarray is a contiguous part of an array.  
Example 1: Input: nums = [-2,1,-3,4,-1,2,1,-5,4] Output: 6  
Explanation: [4,-1,2,1] has the largest sum = 6.  
Example 2: Input: nums = [1] Output: 1  
Example 3: Input: nums = [5,4,-1,7,8] Output: 23  
Constraints:  
1 <= nums.length <= 105  
-104 <= nums[i] <= 104  
I first told him O(n^2) solution. He asked more efficient approach.  
I gave the solution using sliding window approach. He told me to write the code in any my preferred language. After that he give me one test case and asked to dry run my solution on the test case and explain him step by step.

Q2: You are climbing a staircase. It takes n steps to reach the top. Each time you can either climb 1 or 2 steps. In how many distinct ways can you climb to the top?  
Example 1: Input: n = 2 Output: 2  
Explanation: There are two ways to climb to the top.  
Example 2: Input: n = 3 Output: 3  
Explanation: There are three ways to climb to the top.  
Constraints:  
1 <= n <= 45  
I started to give an approach but going wrong direction. He told me first to explain what will be the output for input 4 and 5 in brute-force solution. I show him what combinations are possible for input 4 and 5. Then I was able to catch it that it was a Fibonacci series. He asked me to first write the code in recursive method and explain him the complexity of recursive approach. Then give him the more improved approach and compare between the approaches and what are advantages and disadvantages.

Q3: Lastly he asked me to write example of some sql queries.

1. Ascending and descending order
2. Group by and aggregate function

The whole interview was around 30 minutes long.  
On the same day, evening they called me to inform that the next interview will be taken the very next day.

---

**Round 2 ( Problem Solving + LLD - taken by senior developer ) - ( Lean Hire / Reject ) **

DSA: [https://leetcode.com/problems/reverse-integer/description/](https://leetcode.com/problems/reverse-integer/description/) ( wasn't able to solve this as I got a bit panicked. Hence, lean hire/reject )  
LLD: Factory Pattern implementation  
Grilled a lot on Java features ex how garbage collection works ? what's new in java 8/11/17 ? Funtional Interface etc and gave few scenarios to which needs to be implemented via stream api etc.

---

1. The interviewer appeared disinterested and was more keen on talking about his prowess as SDE in test at Microsoft 15 years back and how he became a program manager. He lamented about how these days everyone memorizes solutions from leetcode and how he is so smart. He asked a lame supposedly OO question. When the answer was provided he kept changing the question to something different. Wanted to say that is called preparation - but he seemed to have an axe to grind and was blabbering about old days, like he was the decision maker - may be he was. Very condescending attitude. From my past experience, I have seen a few other types of these people at Oracle - who gave this vibe like - like this country belongs to us and who are you - type of feeling.

---

Day1  
Round1 - White board, coding. Implement special linked list with Fixed Array as data in node. Implent get, add methods  
Round2 - Enhance existing job search system, Get list of top of jobs which available recruuiter balance, Recruiter pays per click changes by time.  
30mins break  
Round3 - Resume deep dive, Behavioural

----
