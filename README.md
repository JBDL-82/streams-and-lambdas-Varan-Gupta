# 🎯 streams-and-lambdas-assignment


### **Objective**
This assignment is designed to help you gain hands-on experience with the **Java Stream API**. You will write functional-style code to solve real-world data processing problems.

---

### 📌 **Instructions**
- Use **Java Streams** for all solutions unless otherwise stated.
- Do not use traditional loops (`for`, `while`, etc.) unless required.
- Create a separate Java class for each question inside the `src/` directory.

---

### ✅ **Assignment Questions**

---

#### **Q1. Filter Employees by Salary**
Given a list of `Employee` objects, return all employees whose salary is greater than 50,000.

```java
class Employee {
    String name;
    double salary;
}
```
Solution:

```java
Employee e1 = new Employee("Varan",500000);
        Employee e2 = new Employee("Karan",3000);
        Employee e3 = new Employee("Sharan",4000000);
        List<Employee> empObj = new ArrayList<>();
        empObj.add(e1);
        empObj.add(e2);
        empObj.add(e3);
empObj.stream()
        .filter(x-> x.salary > 50000)
        .map(x-> x.name)
        .forEach(x -> System.out.println(x));
```
---

#### **Q2. Word Frequency Counter**
Given a list of words, return a map with the frequency of each word.

```java
Input: ["apple", "banana", "apple"]
Output: {apple=2, banana=1}
```
```java
List<String> words = Arrays.asList("apple", "banana", "apple");
Map<String, Integer> MapObj = new HashMap<>();
        
words.stream()
  .forEach(x-> MapObj.put(x, MapObj.getOrDefault(x,0) + 1));
```
---

#### **Q3. Group Employees by Department**
Group a list of employees by their department.

```java
class Employee {
    String name;
    String department;
}
```

---

#### **Q4. Employee with Max Salary**
Find the employee with the highest salary from the list.

---

#### **Q5. Join Strings with Comma**
Join all strings in a list using a comma as a delimiter.

```java
Input: ["Java", "Python", "C++"]
Output: "Java,Python,C++"
```

---

#### **Q6. Remove Duplicate Elements**
Remove all duplicates from a list of integers.

---

#### **Q7. Partition Employees by Experience**
Given a list of employees, partition them into two groups:  
- Experience >= 5 years  
- Experience < 5 years

```java
class Employee {
    String name;
    int experience;
}
```

---

#### **Q8. Average Salary by Department**
Return a map of department → average salary.

---

#### **Q9. Top 3 Salaries**
Return the names of the top 3 highest-paid employees.

---

#### **Q10. Sort Employees by Salary (Descending)**
Return the list of employees sorted by salary in descending order.

---

#### **Q11. Departments with No Employees**
Given a list of departments and a list of employees, return the names of departments with **no employees assigned**.

---

#### **Q12. Employee Name Initial Map**
Return a map where the key is the **first character** of employee names, and the value is a list of names starting with that character.

```java
Input: ["Alice", "Andrew", "Bob"]
Output: {A=[Alice, Andrew], B=[Bob]}
```

---


### 🚀 Submission Guidelines
- Submit your completed code through your **GitHub Classroom repository**.
