# Operators in C# 🚀

## Introduction

Operators are special symbols used to perform operations on variables and values.

Operators help us:
- perform calculations
- compare values
- apply conditions
- create program logic

Operators are used in almost every C# application.

---

# Why Operators Are Important?

- Perform mathematical calculations
- Build conditions and validations
- Create application logic
- Used in loops, conditions, and APIs
- Essential for ASP.NET Core development

---

# Real-Life Example

Think of operators like tools.

- `+` → calculator addition
- `==` → comparison
- `&&` → checking multiple conditions

Example:
A login system may check:

```csharp
username == "admin" && password == "123"
```

---

# Types of Operators in C#

| Operator Type | Purpose |
|---|---|
| Arithmetic Operators | Mathematical operations |
| Assignment Operators | Assign values |
| Comparison Operators | Compare values |
| Logical Operators | Combine conditions |
| Increment/Decrement Operators | Increase or decrease values |

---

# 1. Arithmetic Operators

Arithmetic operators are used for mathematical calculations.

| Operator | Meaning | Example |
|---|---|---|
| + | Addition | a + b |
| - | Subtraction | a - b |
| * | Multiplication | a * b |
| / | Division | a / b |
| % | Modulus (Remainder) | a % b |

---

# Arithmetic Example

```csharp
using System;

class Program
{
    static void Main()
    {
        int a = 10;
        int b = 5;

        Console.WriteLine("Addition: " + (a + b));
        Console.WriteLine("Subtraction: " + (a - b));
        Console.WriteLine("Multiplication: " + (a * b));
        Console.WriteLine("Division: " + (a / b));
        Console.WriteLine("Modulus: " + (a % b));
    }
}
```

---

# Output

```txt
Addition: 15
Subtraction: 5
Multiplication: 50
Division: 2
Modulus: 0
```

---

# 2. Assignment Operators

Assignment operators assign values to variables.

| Operator | Example | Meaning |
|---|---|---|
| = | a = 10 | Assign value |
| += | a += 5 | Add and assign |
| -= | a -= 5 | Subtract and assign |
| *= | a *= 5 | Multiply and assign |
| /= | a /= 5 | Divide and assign |

---

# Assignment Example

```csharp
int number = 10;

number += 5;

Console.WriteLine(number);
```

Output:

```txt
15
```

---

# 3. Comparison Operators

Comparison operators compare two values.

| Operator | Meaning |
|---|---|
| == | Equal to |
| != | Not equal to |
| > | Greater than |
| < | Less than |
| >= | Greater than or equal |
| <= | Less than or equal |

---

# Comparison Example

```csharp
int age = 20;

Console.WriteLine(age >= 18);
```

Output:

```txt
True
```

---

# 4. Logical Operators

Logical operators combine multiple conditions.

| Operator | Meaning |
|---|---|
| && | AND |
| || | OR |
| ! | NOT |

---

# Logical Example

```csharp
bool hasID = true;
bool hasTicket = true;

Console.WriteLine(hasID && hasTicket);
```

Output:

```txt
True
```

---

# 5. Increment and Decrement Operators

Used to increase or decrease values.

| Operator | Meaning |
|---|---|
| ++ | Increment |
| -- | Decrement |

---

# Example

```csharp
int count = 5;

count++;

Console.WriteLine(count);
```

Output:

```txt
6
```

---

# Real-World Usage

Operators are used in:
- login systems
- validations
- calculations
- loops
- conditions
- APIs
- ASP.NET Core applications

Example:

```csharp
int marks = 85;

bool isPass = marks >= 35;

Console.WriteLine(isPass);
```

---

# Important Notes

- `=` is assignment operator
- `==` is comparison operator
- Logical operators are heavily used in conditions
- `%` gives remainder value

---

# Interview Questions

## Q1. Difference between = and == ?

| = | == |
|---|---|
| Assign value | Compare value |

---

## Q2. What is modulus operator?

The modulus operator `%` returns the remainder after division.

Example:

```csharp
10 % 3 = 1
```

---

## Q3. Difference between && and || ?

| && | || |
|---|---|
| Both conditions must be true | At least one condition must be true |

---




---

# What I Learned Today

- Learned different types of operators
- Practiced arithmetic operations
- Understood comparison and logical operators
- Learned real-world operator usage

---



### Umang Busa
ASP.NET Core Developer Journey 🚀
