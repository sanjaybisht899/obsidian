
---

## IC3 R3

```java 
String s="Hello World";

s=s.lowerCase();

int []arr = new int[26];

int max=0;
int index=0;
char result;
for(char a:s){
	index= a -'a';
	if(index>=0 && index<=26){
		arr[index]++;
		if(max<arr[index]){
			max=arr[index];
			result=a;
		}
	}
	
}

HashMap<Character,Integer> map = new HashMap<>();

int max=0;
char result;
for(char a:s){
	map.put(a,map.getOrDefault(a,0)+1);
	if(max<map.get(a)){
		max=map.get(a);
		result=a;
	}
}


for(Map.Entry<Character,Integer> entry : map.entrySet()){
	System.out.println(entry.getKey()+" : "entry.getValue());
}

String s="Hello World";


//Reverse the string using stack
//abc
c
b
a

Stack<Character> stack = new Stack<>();

for(char a : s.toCharArray()){
	stack.push(a);
}

StringBuilder str = new StringBuilder();

while(!stack.isEmpty()){
	str.append(stack.pop());

	//s=s+stack.pop();
}

str.toString();




sychronized(lock){
	
}



Singleton class



class Singleton{
	//synchronozed

	private static Singleton singleton;
	private Singleton(){}
	public static Singleton getInstance(){
		if(singleton == null){
			synchronozed(Singleton.class){
				if(singleton == null){
					singleton = new Singleton();
				}
			}
		}
		return singleton;
	}
}

Department 

Each employee belong a department

each employee


------------------
EmpID, Name, DepID
               


---------
DeptID, Name



----

Write a query to find all departments with more than 10 employees

SELECT d.Name, COUNT(e.EmpID) as Count
FROM DEPARTMENT d
JOIN Employee e ON d.DeptID = e.DeptID
GROUP BY d.NAME
HAIVNG COUNT(e.EmpID)> 10;

Write a query to fetch all the employees who work for a particular department


SELECT e.NAME 
FROM Department d
JOIN Employee e ON d.DeptID = e.DeptID 
WHERE d.NAME="HR" ORDER BY e.NAME ASC;


























































