# PROG5121 POE Part 3: Guided Activities

## Overview

Part 3 focuses on the following programming concepts:

- Arrays and Parallel Arrays
- Searching Arrays
- String Manipulation
- Reading JSON Data
- Menu-Driven Applications
- Data Reports

The activities below are designed to help you build the final solution incrementally.

---

# Activity 1: Creating Parallel Arrays

## Objective
Learn how related data can be stored using parallel arrays.

## Task
Create the following arrays:

```java
String[] recipients = new String[5];
String[] messages = new String[5];
String[] statuses = new String[5];
```

Populate the first message:

```java
recipients[0] = "+27834557896";
messages[0] = "Did you get the cake?";
statuses[0] = "Sent";
```

## Challenge

Use a loop to display all messages currently stored in the arrays.

### Expected Output

```
Recipient: +27834557896
Message: Did you get the cake?
Status: Sent
```

## Resource

W3Schools Java Arrays:

https://www.w3schools.com/java/java_arrays.asp

---

# Activity 2: Searching an Array

## Objective

Search for a recipient number within an array.

## Task

Prompt the user to enter a recipient number:

```java
Scanner scanner = new Scanner(System.in);

System.out.print("Enter recipient: ");
String searchRecipient = scanner.nextLine();
```

Search the recipient array and display all matching messages.

### Test Input

```
+27838884567
```

### Expected Output

```
Where are you? You are late! I have asked you to be on time.
Ok, I am leaving without you.
```

## Resource

GeeksForGeeks – Searching in Arrays:

 https://www.geeksforgeeks.org/java/how-to-get-first-element-in-array-in-java/

---

# Activity 3: Finding the Longest Message

## Objective

Use loops and string methods to identify the longest message.

## Task

Determine which message contains the greatest number of characters.

### Hint

```java
message.length()
```

### Expected Output

```
Where are you? You are late! I have asked you to be on time.
```

## Resource

W3Schools String Length:

https://www.w3schools.com/java/ref_string_length.asp

---

# Activity 4: Search by Message ID

## Objective

Search parallel arrays using a Message ID.

## Task

Ask the user to enter a Message ID.

### Test Input

```
0838884567
```

### Expected Output

```
Recipient: 0838884567
Message: It is dinner time!
```

## Hint

Use the Message ID array to find the index, then use the same index to retrieve values from the other arrays.

## Resource

Programiz Linear Search:

https://www.programiz.com/dsa/linear-search

---

# Activity 5: Creating a Message Report

## Objective

Generate a formatted report using array data.

## Task

Display all sent messages in the following format:

### Expected Output

```
Message Hash: AB:1:HELLOWORLD
Recipient: +27834557896
Message: Did you get the cake?

Message Hash: CD:2:ITDINNER
Recipient: 0838884567
Message: It is dinner time!
```

## Resource

StringBuilder Tutorial:

https://www.geeksforgeeks.org/java/stringbuilder-class-in-java-with-examples/

---

# Activity 6: Delete a Message Using a Message Hash

## Objective

Modify array data by removing a message.

## Task

Search for a message hash entered by the user.

### Example Input

```
+2:1:WHERETIME
```

If found:

```java
messages[index] = null;
```

### Expected Output

```
Message successfully deleted.
```

## Extension

Display the remaining messages after the deletion.

## Resource

JavaTPoint Arrays:

https://www.tutorialspoint.com/java/java_arrays.htm

---

# Activity 7: Reading Stored Messages from JSON

## Objective

Load stored messages from a JSON file into arrays.

## Task

Create a JSON file named:

```
stored_messages.json
```

### Example JSON

```json
[
  {
    "messageID": "+27838884567",
    "recipient": "+27838884567",
    "message": "Where are you? You are late! I have asked you to be on time.",
    "status": "Stored"
  }
]
```

Read the file and store the values into your arrays.

### Expected Output

```
Stored message loaded successfully.
```

## Resources

JSON Simple Tutorial:

https://mkyong.com/java/json-simple-how-to-parse-json/

JSON Introduction:

https://www.w3schools.com/js/js_json_intro.asp

---

# Activity 8: Build a Menu System

## Objective

Combine all Part 3 features into a menu-driven application.

## Task

Create a menu using Scanner.

### Example Menu

```text
1. Display Sent Messages
2. Display Longest Message
3. Search by Message ID
4. Search by Recipient
5. Delete by Message Hash
6. Display Report
7. Exit
```

Use a loop so that the menu continues to display until the user chooses Exit.

---

# Recommended Learning Resources

## Oracle Java Tutorials

https://docs.oracle.com/javase/tutorial/

## W3Schools Java

https://www.w3schools.com/java/

## GeeksForGeeks Java Arrays

https://www.geeksforgeeks.org/java/arrays-in-java/

## Programiz Java Programming

https://www.programiz.com/java-programming

## JSON Simple Tutorial

https://mkyong.com/java/json-simple-how-to-parse-json/


## JUnit 5 Testing

https://www.baeldung.com/junit-5

---

By completing these activities, you will have implemented every major requirement for Part 3 of the POE.
