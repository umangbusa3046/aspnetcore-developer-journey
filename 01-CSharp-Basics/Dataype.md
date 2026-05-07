# Data Types in C# 🚀

## Introduction

Data types define what kind of data a variable can store.

In C#, every variable must have a data type.

Data types help:
- store data properly
- manage memory efficiently
- perform operations correctly

---

# Why Data Types Are Important?

- Improve performance
- Prevent invalid data storage
- Make code more organized
- Used in every application

---

# Real-Life Example

Think of data types like different containers.

- Water bottle → stores water
- Lunch box → stores food
- Wallet → stores money

Similarly:
- `int` stores numbers
- `string` stores text
- `bool` stores true/false

---

# Common Data Types in C#

| Data Type | Description | Example |
|---|---|---|
| int | Integer numbers | 10 |
| double | Decimal numbers | 10.5 |
| float | Small decimal numbers | 12.3f |
| decimal | High precision decimal | 99.99m |
| char | Single character | 'A' |
| string | Text | "Umang" |
| bool | True or False | true |

---

# Syntax

```csharp
datatype variableName = value;
```

Example:

```csharp
int age = 21;
string name = "Umang";
```

---

# Example Program

```csharp
using System;

class Program
{
    static void Main()
    {
        int age = 21;
        double percentage = 85.5;
        char grade = 'A';
        string name = "Umang";
        bool isPlaced = false;

        Console.WriteLine("Name: " + name);
        Console.WriteLine("Age: " + age);
        Console.WriteLine("Percentage: " + percentage);
        Console.WriteLine("Grade: " + grade);
        Console.WriteLine("Placed: " + isPlaced);
    }
}
```

---

# Output

```txt
Name: Umang
Age: 21
Percentage: 85.5
Grade: A
Placed: False
```

---

# Explanation

| Code | Explanation |
|---|---|
| int age = 21; | Stores integer value |
| double percentage = 85.5; | Stores decimal value |
| char grade = 'A'; | Stores single character |
| string name = "Umang"; | Stores text |
| bool isPlaced = false; | Stores true/false |

---

# Value Types vs Reference Types

## Value Types

Store actual values directly.

Examples:
- int
- double
- bool
- char

---

## Reference Types

Store memory address of the object.

Examples:
- string
- array
- class

---

# Difference Between float, double, and decimal

| Type | Precision | Use Case |
|---|---|---|
| float | Low | Graphics |
| double | Medium | General calculations |
| decimal | High | Financial calculations |

---

# Important Notes

- C# is case-sensitive
- Variable names should be meaningful
- Every variable must have a data type
- Initialize variables before use

---

# Interview Questions

## Q1. What is a data type in C#?

A data type defines the kind of value a variable can store.

---

## Q2. Difference between int and double?

| int | double |
|---|---|
| Stores whole numbers | Stores decimal numbers |

---

## Q3. Difference between value type and reference type?

| Value Type | Reference Type |
|---|---|
| Stores actual data | Stores memory address |
| Faster | Slightly slower |

---




# What I Learned Today

- Learned different C# data types
- Understood value and reference types
- Practiced variable declaration
- Learned real-world usage of data types

---

### Umang Busa
ASP.NET Core Developer Journey 🚀
