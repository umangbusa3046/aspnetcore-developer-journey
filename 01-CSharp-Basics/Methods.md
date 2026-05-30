# Methods (Functions) in C# 🚀

## Introduction

A method is a reusable block of code that performs a specific task.

Methods help developers:

- Avoid code duplication
- Improve code readability
- Organize business logic
- Make applications easier to maintain

Methods are one of the most important concepts in C# and are used extensively in ASP.NET Core applications.

---

# Why Methods Are Important?

Without methods, we would need to write the same code repeatedly.

Benefits:

- Reusability
- Better organization
- Easier debugging
- Improved maintainability
- Cleaner code structure

---

# Real-Life Example

Think of a method like a coffee machine.

When you press a button:

```txt
MakeCoffee()
```

The machine performs multiple internal steps and gives you coffee.

You don't need to know every internal process each time.

Similarly, a method performs a task whenever it is called.

---

# What is a Method?

A method is a named block of code that can:

- Perform a task
- Accept input
- Return output
- Be reused multiple times

---

# Method Syntax

```csharp
access_modifier return_type MethodName()
{
    // code
}
```

Example:

```csharp
static void DisplayMessage()
{
    Console.WriteLine("Welcome to C#");
}
```

---

# Parts of a Method

```csharp
static int Add(int a, int b)
{
    return a + b;
}
```

| Part | Description |
|--------|------------|
| static | Method belongs to the class |
| int | Return type |
| Add | Method name |
| int a, int b | Parameters |
| return | Sends value back |

---

# 1. Void Method

A void method performs a task but does not return any value.

---

# Example

```csharp
using System;

class Program
{
    static void DisplayMessage()
    {
        Console.WriteLine("Welcome to C#");
    }

    static void Main()
    {
        DisplayMessage();
    }
}
```

---

# Output

```txt
Welcome to C#
```

---

# Explanation

| Code | Meaning |
|--------|----------|
| void | No value returned |
| DisplayMessage() | Method name |
| Console.WriteLine() | Displays output |

---

# 2. Method with Parameters

Parameters allow methods to receive data.

---

# Example

```csharp
using System;

class Program
{
    static void Greet(string name)
    {
        Console.WriteLine("Hello " + name);
    }

    static void Main()
    {
        Greet("Umang");
    }
}
```

---

# Output

```txt
Hello Umang
```

---

# Explanation

| Item | Value |
|--------|--------|
| Parameter | name |
| Argument | "Umang" |

---

# Parameter vs Argument

| Parameter | Argument |
|------------|-----------|
| Defined in method | Passed during method call |
| Placeholder | Actual value |

Example:

```csharp
void Greet(string name)
```

`name` = Parameter

```csharp
Greet("Umang");
```

`"Umang"` = Argument

---

# 3. Method Returning a Value

A return method sends data back to the caller.

---

# Example

```csharp
using System;

class Program
{
    static int Add(int a, int b)
    {
        return a + b;
    }

    static void Main()
    {
        int result = Add(10, 20);

        Console.WriteLine(result);
    }
}
```

---

# Output

```txt
30
```

---

# Explanation

| Code | Meaning |
|--------|----------|
| int | Returns integer |
| return a + b | Sends result back |
| result | Stores returned value |

---

# Common Return Types

| Return Type | Meaning |
|------------|----------|
| void | No return value |
| int | Integer |
| double | Decimal |
| string | Text |
| bool | True or False |
| char | Single character |

---

# 4. Method Overloading

Method overloading allows multiple methods with the same name but different parameters.

---

# Example

```csharp
using System;

class Program
{
    static int Add(int a, int b)
    {
        return a + b;
    }

    static int Add(int a, int b, int c)
    {
        return a + b + c;
    }

    static void Main()
    {
        Console.WriteLine(Add(10, 20));
        Console.WriteLine(Add(10, 20, 30));
    }
}
```

---

# Output

```txt
30
60
```

---

# Why Method Overloading?

Benefits:

- Cleaner code
- Better readability
- Reuse method names

---

# Complete Example

```csharp
using System;

class Program
{
    static void DisplayMessage()
    {
        Console.WriteLine("Welcome to C#");
    }

    static void Greet(string name)
    {
        Console.WriteLine("Hello " + name);
    }

    static int Add(int a, int b)
    {
        return a + b;
    }

    static bool IsEligibleToVote(int age)
    {
        return age >= 18;
    }

    static void Main()
    {
        DisplayMessage();

        Greet("Umang");

        Console.WriteLine("Sum: " + Add(10, 20));

        Console.WriteLine("Eligible: " + IsEligibleToVote(21));
    }
}
```

---

# Output

```txt
Welcome to C#
Hello Umang
Sum: 30
Eligible: True
```

---

# Real-World Usage

Methods are used everywhere in ASP.NET Core:

### Controller Method

```csharp
public IActionResult GetStudents()
{
    return View();
}
```

### Service Method

```csharp
public List<Student> GetAllStudents()
{
    return students;
}
```

### Repository Method

```csharp
public Student GetStudentById(int id)
{
    return student;
}
```

---

# Advantages of Methods

- Reusable code
- Easier maintenance
- Better readability
- Reduced duplication
- Easier testing

---

# Important Notes

- Method names should be meaningful
- Follow PascalCase naming convention
- Use parameters when input is needed
- Use return types when output is needed
- Avoid writing large methods

---

# Interview Questions

## Q1. What is a method?

A reusable block of code that performs a specific task.

---

## Q2. Difference between parameter and argument?

| Parameter | Argument |
|------------|-----------|
| Defined in method | Passed while calling |

---

## Q3. Difference between void and return?

| void | return |
|------|--------|
| Returns nothing | Returns a value |

---

## Q4. What is method overloading?

Using the same method name with different parameter lists.

---

## Q5. Can a method return multiple values?

Yes, using:

- Tuple
- out parameters
- objects/classes

---

# Practice Tasks

## Task 1

Create a method:

```csharp
DisplayName()
```

Print your name.

---

## Task 2

Create a method:

```csharp
Multiply(int a, int b)
```

Return multiplication result.

---

## Task 3

Create a method:

```csharp
IsEligibleToVote(int age)
```

Return:

```csharp
true
```

or

```csharp
false
```

based on age.

---

# Mini Project

## Student Utility Program

Create methods:

```csharp
DisplayStudent()
CalculatePercentage()
CheckPassFail()
```

Use:

- Methods
- Parameters
- Return Types
- Conditions

---

# What I Learned Today

- Learned what methods are
- Understood method syntax
- Practiced parameters and arguments
- Learned return types
- Understood method overloading
- Learned real-world ASP.NET Core usage

---



## Umang Busa
ASP.NET Core Developer Journey 🚀
