# Conditions & Looping in C# 🚀

## Introduction

Conditions and loops control the flow of a program.

- Conditions help programs make decisions.
- Loops help programs repeat tasks efficiently.

These concepts are fundamental in every programming language and heavily used in real-world applications.

---

# Why Conditions & Loops Are Important?

They help programs:

- Make decisions based on data
- Repeat tasks automatically
- Process collections and lists
- Validate input
- Build dynamic applications

Without conditions and loops, applications would not be interactive or scalable.

---

# Real-World Examples

## Conditions

- Login validation
- Age eligibility checks
- Grade calculation
- Payment status handling

---

## Loops

- Processing customer orders
- Reading database records
- Displaying product lists
- Retrying failed network requests

---

# 1. if / else Statement

Used to execute code based on conditions.

---

# Syntax

```csharp
if(condition)
{
    // code
}
else
{
    // code
}
```

---

# Example

```csharp
int score = 85;

if (score >= 90)
{
    Console.WriteLine("Grade: A");
}
else if (score >= 75)
{
    Console.WriteLine("Grade: B");
}
else
{
    Console.WriteLine("Grade: C or Below");
}
```

---

# Output

```txt
Grade: B
```

---

# Explanation

| Condition | Result |
|---|---|
| score >= 90 | Grade A |
| score >= 75 | Grade B |
| Otherwise | Grade C |

---

# 2. switch Statement

Used when there are multiple fixed choices.

---

# Syntax

```csharp
switch(variable)
{
    case value:
        // code
        break;

    default:
        // code
        break;
}
```

---

# Example

```csharp
string command = "start";

switch (command)
{
    case "start":
        Console.WriteLine("Started");
        break;

    case "stop":
        Console.WriteLine("Stopped");
        break;

    default:
        Console.WriteLine("Unknown Command");
        break;
}
```

---

# Output

```txt
Started
```

---

# Why switch is Useful?

- Cleaner than multiple if-else statements
- Easier to read
- Better for menu-driven applications

---

# 3. for Loop

Used when the number of repetitions is known.

---

# Syntax

```csharp
for(initialization; condition; increment/decrement)
{
    // code
}
```

---

# Example

```csharp
for (int i = 0; i < 3; i++)
{
    Console.WriteLine($"for: {i}");
}
```

---

# Output

```txt
for: 0
for: 1
for: 2
```

---

# Explanation

| Part | Purpose |
|---|---|
| int i = 0 | Starting value |
| i < 3 | Condition |
| i++ | Increment |

---

# 4. while Loop

Used when repetitions depend on a condition.

---

# Syntax

```csharp
while(condition)
{
    // code
}
```

---

# Example

```csharp
int n = 3;

while (n-- > 0)
{
    Console.WriteLine($"while: {n}");
}
```

---

# Output

```txt
while: 2
while: 1
while: 0
```

---

# Why while Loop is Useful?

- User input validation
- Retry mechanisms
- Running tasks until condition becomes false

---

# 5. do-while Loop

Executes code at least once.

---

# Syntax

```csharp
do
{
    // code
}
while(condition);
```

---

# Example

```csharp
int number = 1;

do
{
    Console.WriteLine(number);
    number++;
}
while(number <= 3);
```

---

# Output

```txt
1
2
3
```

---

# Difference Between while and do-while

| while | do-while |
|---|---|
| Checks condition first | Executes first |
| May execute zero times | Executes at least once |

---

# 6. foreach Loop

Used to iterate collections easily.

---

# Example

```csharp
using System.Collections.Generic;

var names = new List<string>
{
    "Alice",
    "Bob",
    "Charlie"
};

foreach (var name in names)
{
    Console.WriteLine($"Hello {name}");
}
```

---

# Output

```txt
Hello Alice
Hello Bob
Hello Charlie
```

---

# Why foreach is Useful?

- Cleaner syntax
- Safer iteration
- Best for collections and arrays

---

# Complete Example Program

```csharp
using System;
using System.Collections.Generic;

class Program
{
    static void Main()
    {
        int score = 85;

        // if / else
        if (score >= 90)
            Console.WriteLine("Grade: A");
        else if (score >= 75)
            Console.WriteLine("Grade: B");
        else
            Console.WriteLine("Grade: C or below");

        // switch
        string command = "start";

        switch (command)
        {
            case "start":
                Console.WriteLine("Started");
                break;

            case "stop":
                Console.WriteLine("Stopped");
                break;

            default:
                Console.WriteLine("Unknown command");
                break;
        }

        // for loop
        for (int i = 0; i < 3; i++)
            Console.WriteLine($"for: {i}");

        // while loop
        int n = 3;

        while (n-- > 0)
            Console.WriteLine($"while: {n}");

        // foreach loop
        var names = new List<string>
        {
            "Alice",
            "Bob",
            "Charlie"
        };

        foreach (var name in names)
            Console.WriteLine($"Hello {name}");
    }
}
```

---

# Use Cases

## Conditions

- Authentication systems
- Role-based access
- Form validation
- API response handling

---

## Loops

- Database processing
- Reading files
- API pagination
- Data migration
- Batch operations

---

# Important Notes

- Use `if-else` for dynamic conditions
- Use `switch` for fixed choices
- Use `for` when count is known
- Use `while` when condition-based repetition is needed
- Use `foreach` for collections

---

# Interview Questions

## Q1. Difference between if-else and switch?

| if-else | switch |
|---|---|
| Works with complex conditions | Works with fixed values |
| More flexible | Cleaner for multiple choices |

---

## Q2. Difference between for and foreach?

| for | foreach |
|---|---|
| Uses index | Direct iteration |
| More control | Simpler and safer |

---

## Q3. Difference between while and do-while?

| while | do-while |
|---|---|
| Condition checked first | Executes first |
| May not execute | Executes at least once |

---

# Mini Practice Tasks

---

# Task 1 — Print Even Numbers from 1 to 20

## Problem Statement

Print all even numbers from 1 to 20 using a `for` loop.

---

# Solution

```csharp
using System;

class Program
{
    static void Main()
    {
        for (int i = 1; i <= 20; i++)
        {
            if (i % 2 == 0)
            {
                Console.WriteLine(i);
            }
        }
    }
}
```

---

# Output

```txt
2
4
6
8
10
12
14
16
18
20
```

---

# Explanation

| Code | Meaning |
|---|---|
| for loop | Repeats from 1 to 20 |
| i % 2 == 0 | Checks even number |
| Console.WriteLine() | Prints output |

---

# Important Concept

## Modulus Operator `%`

Returns remainder after division.

Example:

```csharp
10 % 2 = 0
```

If remainder is `0`, the number is even.

---

# Task 2 — Sum Numbers Until User Enters 0

## Problem Statement

Read numbers from the user until the user enters `0`.

Print the total sum using a `while` loop.

---

# Solution

```csharp
using System;

class Program
{
    static void Main()
    {
        int number;
        int sum = 0;

        Console.WriteLine("Enter numbers (0 to stop):");

        while (true)
        {
            number = Convert.ToInt32(Console.ReadLine());

            if (number == 0)
            {
                break;
            }

            sum += number;
        }

        Console.WriteLine("Total Sum: " + sum);
    }
}
```

---

# Example Output

```txt
Enter numbers (0 to stop):

5
10
15
0

Total Sum: 30
```

---

# Explanation

| Code | Meaning |
|---|---|
| while(true) | Infinite loop |
| break | Stops loop |
| sum += number | Adds number to sum |

---

# Real-World Use Case

This logic is used in:
- billing systems
- cart totals
- financial calculations
- data aggregation

---

# Bonus Challenge — Menu Driven Calculator

## Problem Statement

Create a calculator using:
- switch
- loops
- conditions

Operations:
- Addition
- Subtraction
- Multiplication
- Division

---

# Solution

```csharp
using System;

class Program
{
    static void Main()
    {
        bool running = true;

        while (running)
        {
            Console.WriteLine("\n===== Calculator Menu =====");
            Console.WriteLine("1. Addition");
            Console.WriteLine("2. Subtraction");
            Console.WriteLine("3. Multiplication");
            Console.WriteLine("4. Division");
            Console.WriteLine("5. Exit");

            Console.Write("Choose Option: ");

            int choice = Convert.ToInt32(Console.ReadLine());

            if (choice == 5)
            {
                running = false;
                Console.WriteLine("Calculator Closed");
                break;
            }

            Console.Write("Enter First Number: ");
            double num1 = Convert.ToDouble(Console.ReadLine());

            Console.Write("Enter Second Number: ");
            double num2 = Convert.ToDouble(Console.ReadLine());

            switch (choice)
            {
                case 1:
                    Console.WriteLine("Result: " + (num1 + num2));
                    break;

                case 2:
                    Console.WriteLine("Result: " + (num1 - num2));
                    break;

                case 3:
                    Console.WriteLine("Result: " + (num1 * num2));
                    break;

                case 4:

                    if (num2 != 0)
                    {
                        Console.WriteLine("Result: " + (num1 / num2));
                    }
                    else
                    {
                        Console.WriteLine("Cannot divide by zero");
                    }

                    break;

                default:
                    Console.WriteLine("Invalid Choice");
                    break;
            }
        }
    }
}
```

---

# Example Output

```txt
===== Calculator Menu =====

1. Addition
2. Subtraction
3. Multiplication
4. Division
5. Exit

Choose Option: 1

Enter First Number: 10
Enter Second Number: 20

Result: 30
```

---

# Concepts Used

| Concept | Usage |
|---|---|
| if | Validation |
| switch | Menu options |
| while loop | Continuous execution |
| break | Exit loop |
| arithmetic operators | Calculations |

---

# Real-World Use Case

Menu-driven systems are used in:
- ATM machines
- Restaurant systems
- Admin panels
- Console tools
- Inventory systems

---

# What I Learned

- Practiced loops deeply
- Understood condition handling
- Used switch statements
- Built a real calculator
- Learned input validation

---

### Umang Busa
ASP.NET Core Developer Journey 🚀
