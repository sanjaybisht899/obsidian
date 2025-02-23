
---


System Design - Similar to Inventory Management  
Requirements:

1. clients are store owners
2. clients should be able to place orders with 3rd party vendors(external api)

- i started off nice, gathered functional, non-functional etc
- i asked him if i'm good to start, he said ok
- but, when i started api section, he asked how can clients view the products? (i missed it in the functional reqs, so i added it)
- i came up with some high level design with single components i.e. server, db
- he stopped me at last 15 mins saying, need time for behavioral and asked me if i want to add anything to the design, so, i mentioned i would use a queue between inventory management system and the external api, gave reasons for what type of db, cache i would choose
- he did not ask me any other questions during the system design other than that 1 functional req i missed
- i'm not sure if this round went well as interviewer did not hint anything & he stopped me even before i finished my design

Behavioral

1. any procedure or process that you've improved in your team
2. foreseen a bug & fixed it

---
- Behavioral questions: **"Why do you want to join Oracle?"**, etc.


---
**Round 5 ( Culter Fit round - taken by another team's manager ) ** - ( Hire )

Standard questions like:  
What happens during a clash over design ? How would you resolve that  
What is the reason for changing company ?  
Any project which have completely taken care from scratch ?  
Any mentoring which you did during your stint ?

---
Round 5: Mangerial Round

- Explain HLD of your project
- How did you manage timelines in your project?
- How did you mentor junior engineer?

---
Round 4: Bar raiser round

- We have a gaming scoreboard .
    
- Design APIs/methods for provide score dashboard for a game.
    
- Feature Requirements:
    
    - #1 Fetch score/player details of current player by Name or Id.
    - #2 UpdateOrCreate score of player by Name or Id.
    - #3 Fetch player details with highest score
    - #4 Fetch leaderboard, dashboard in DES order (score).
    - #5 Delete the player
- Assumptions:
    
    - Names are unique (simplification)
    - Use Data-structures instead of DB

Behavorial:

- Can you tell me about a time where you did something outside your area of responsibility ?
- Can you tell me about a time where learned something new,a new tech stack?

---
**Round 3: Hiring Manager**  
After the initial introduction, the panel gave me a design problem: to design an OTT platform like Netflix or Prime Video. I started with requirement gathering, both functional and non-functional, and then did a capacity estimation. It was a very interactive interview. The focus was on how the personalized feeds for users would be designed and how movies and TV shows would be streamed to devices. We had a good debate on push vs. pull CDN approaches and the scalability of the herd problem in case of a popular show release. In the end, the Hiring Manager asked me LP questions. This was my best round.

---
**Third round:** Managerial round  
She was manager. She started with introduction and project grilling.  
Then lot of scenario based question:

1. Any colleage inspires you?
2. Any tech challenge you faced?
3. Any scenario when your boss changed and how you handled?
4. Any scenario when you missed deadline?
5. How you handle priority change?
6. Why switching job?

Coding question : Variation of [https://leetcode.com/problems/merge-intervals/description/](https://leetcode.com/problems/merge-intervals/description/)  
First I gave brute force solution and then most optimised solution.

In the end, she asked if i have any question. Again my bad i ask at what stage oracle cloud is. She replied what do u mean by stage. I replied its with clients or its in Poc. He said you can google its going with full-fledged and have many clients.


---
**Round 3:**

**Managerial Round:**

- Questions about reasons for switching and team fit.
- Project Discussion:
    - Asked about their project and tech stack.
- Asked questions how would you perform load testing
---
**Round 3:** This was just a discussion with the Senior Director and sort of not an interview.

- Here he explained me about the product and the team which I will be a part of, in detail.
- He also explained me the difference b/w a product-based company and a service based company
- He also asked me about my current CTC and said I would get much more than this.




---
In this round, the discussion revolved around my career achievements:

- I shared my major accomplishments at my current employer, and we had an in-depth conversation about the key projects I’ve worked on.
- The interviewer also asked some standard leadership and behavioral questions, which allowed me to showcase my problem-solving and collaboration skills.

---
Round 3 - Round 3: this is where I was grilled on the project, there were some behavioural questions and some based on project, but I really did not understand what exactly the interviewer was looking for, he kept on stopping me and was asking "what you did?" but was not letting me explain anything.  
- This interview was an average for me.

---

(Round 4)- > Open ended (Monitoring and observability) ->  
What monitoring tools I have used.  
How are those tools being used and beneficial.  
How will you design a highly available, scalable and resilient system.  
What caching are used in the project, how caching is beenficial and questions around it.  
What will you do if system goes down how will you handle these scenarios.  
Questions related to networking, what protocols I know and any one used in project (We are using websocket in our project), explained around that.  
Cron jobs and how to handle it if it is not running.  
DB related questions how to improve DB response.  
What to do if cron misses cleaning DB and DB is throttled with full memory.

(Round 5 - Bar tender by IC4) -> It was taken by someone from different team.  
Behavioral questions mostly asked.  
Challeneges faced in current role.  
Any scenario when you were asked to work apart from the given role.  
Any initiative you have taken to improve team performance and communication.  
Any risk you took and it did not go well how do you react to it and your learnings.

Then the questions started with technical side based on my resume regarding the service I developed, what Infra we used and explain use of those infra.  
E2E working of the service.  
How do you decide to use SQS as your messaging queue and not other.  
polling vs eventing mechanism why you moved to eventing based system from polling.

---
**Round 3:**

1. Low Level Design of Key Value Store.
2. Another followup to the 1st Question.
3. Questions on Disk Memory vs In Memory.
4. Few Questions on REST API.

---
**HM Round:**

1. Discussed on the past project.
2. In depth discussion on the search feature that I worked previously as they have a feature in their project too.
3. Questions on day to day activities etc.
4. Overall it is just a normal discussion.

---

**Hiring Manager Round:**

1. Discussion on Past Project
2. Why are you leaving your current company
3. What are your roles and responsibilities at current company
4. Few technical questions on APIs

---
Round 4 - > Taken by Principle Engg Manager (Director )  
Went deep in my project and current work .  
Ask to implement multithreaded event bus (like kafka ) .  
Then had discussions on NQSQL Db . At last fewbehaviour questions and my location prefernce ,  
This round streached til 1.45 hrs .

---

**Round 3:**

- Design a data pipeline where you dump data for each day in s3 storage location and you need to ingest this on incremental basis into oracle db
- How much memory of executors do we need to load 1 tb data
- SQL questions
- Project discussions in-depth
---

**Loop interview 4**(1 hour) -

`4 behavioral questions based on Oracle principles, lots of indepth behavioral question on resume.`  
This was the hiring manager round.

---
Round 5: Discussion around current project and one coding question. Topological sort based question. But needed to print all the nodes which could be sorted and also the nodes which were part of cycle. Got 30 mins for coding question. Could manage only 6 working test cases out of 13.

---
(Round 4 )- > HM Round -> Asked me to code Coin change problem and run all tests .  
Then asked some Behavioral questions , then moved to System design , Discussed deep about NOSQL Database and SAGA Pattern in Microservices .  
AFTER Interview recruiter told Bar tender is not inclined so she wanted me to give one more round which is again Data Structure and System Design .

---
Round 3 - Engineering Manager round

1. Discussion on the tech stack used in the current project. Why Oracle Database and not MySQL Difference between both.
2. Discussion on different Scenarios while dealing with messaging queues.
3. LLD of any type of booking application. He was interested in Classes for Order creation to Order Execution flow.
4. How the design will deal with Different modes of payment system , (Credit Card UPI ) - Explained this using Strategy Design Pattern.
5. Behavioural Questions - Instances when your opinion differed from the rest of the team. What points should be noticed while doing code reviews.

---
## oracle round 3: Taken by hiring manager

- discussion on projects
- my project where I faced challenge
- any time when I had to improve performance
- Various ways to improve performance
- check for palindrome
- next palindrome for a given number

---


Round 3 HM round (zoom call) duration ~1 hour  
- project based dicussion  
- kafka related question as i mentioned kafka  
- redis related question as i mentioned redis in my resume  
- basic encryption/decryption technique  
- SSL vs TLS  
- more project related grills
---
**Round 3** - Managerial Round

- Had an in-depth discussion about the project that I am working on at my org.
- Was asked a Hard Leetcode question. Was able to solve it pretty fast.
- He then asked a follow-up based on coding principles, which I somehow gave a 50-50 answer

---
**Round 5**  
Situation based questions

1. Tell me a situation where you have owned the bug for end to end
2. Indepth explation for project and what are the roles and responsibility
---

**Third Technical Interview**

This was a system design round but they just wanted to discuss about overall concepts and see my approach to common problems. This time the annoying guy returned with the actual manager of the team. He had joined late so the manager had started without him. Manager asked me vague questions like suppose there is some problem with the data of the customer, how will you go about doing RCA. How will you improve the performance of a system? What if the problem is very rare and happening only with some customers etc. Later the other guy joined and started asking the same questions, but manager was kind enough to interrupt and asked him to ask different questions as I had already answered about that. Then, he asked me about Authorization and Authentication, how does oauth, sso work. I didn't know the exact details, but I had a rough idea so I asked for his permission to take a guess, which he refused. Then there were a few more questions related to database and indexing, which i answered.

Recruiter reached out and said that the feedback was average but they wanted to schedule another round with someone from Chile. Later, they cancelled it and went straight to salary discussion. There was another call scheduled with manager and that annoying guy where they asked a few behaviorial questions.

- How do you handle huge workloads?
- Why are you leaving your current position? If you have gotten bored with the work within 3 years, what's the guarantee you will not get bored with our work and leave here soon too?
- What are your thoughts on staying late/ coming in on weekends when there is a specific need?
- Then they asked me to quote my expectation to them, i was a bit surprised as I was used to having this discussion with the recruiter, not the manager (and definitely not that annoying guy staring in my face) but I gave them the number anyway?

Next, they came back for another discussion with a huge lowball. I was extremely disappointed because after so many rounds and asking my expectation even in the beginning, this is what they could come up with? Later, I negotiated with the recruiter and got it up to somewhat decent (still a lowball in my opinion).

---
Round-3 (Hiring Manager Round)  
Structure  
This round was taken by a Sr. SDE from Oracle. The round started with general introduction of interviewer followed by mine. The interviewer told me about the projects he previously worked on and also asked me about the tech stack . This went on for good 10 minutes.

Then for the next 15–20 minutes, I was asked quite a few Leadership Questions and I had to explain different scenarios depicting those Leadership Principles.

For the rest of the interview (30–35 minutes), I was asked Computer Science Fundamentals spanning across topics like Operating System, OOPS, DBMS, DSA etc.

Computer Science Fundamentals

I was asked around 10–15 questions. Some of them are given below:

Object Oriented Programming and its advantages  
Difference between Compositon and Inheritance  
Different types of Scheduling Algorithms  
Critical Section Problem  
Difference between Semaphore and Mutex  
Stored Procedure  
SQL vs NoSQL


---
**Round 4:**  
Hr + few technical ques in OS and DBMS  
OS: Q1. Concurrency vs parallelism?  
Q2. What is a deadlock? Necessary conditions for deadlock to occur?  
Q3. Deadlock avoidance, prevention, removal etc. What is RAG?  
DBMS: Q1. What is normalization and why do we need it?  
Q2. Asked upto BCNF

---
**Loop Round 4 - Hiring Manager**

- Discussion on past projects
- Questions based on resume
- Behavioural questions
---

### echnical Round 3 (45 mins)

- An introduction about me, both technically and non-technically, was requested.
- Explain the different DDL, DML, and DQL commands.
- Solved a DSA question, a Variation of [Find the Index of the First Occurrence in a String](https://leetcode.com/problems/find-the-index-of-the-first-occurrence-in-a-string/description/)
- Discussed Normalization and its purpose.
- Detailed explanation of 2NF and BCNF was asked.
- Was asked to explain all 7 OSI Layers along with associated protocols.
- Explained Multithreading in Java, including codes for Thread and Runnable Interface.
- Discussed Deadlocks and how to detect them.
- What are Semaphores.
- Explain Triggers and PL/SQL
- I asked one question at the end.




---
L1 -- Interviews Here

---

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
