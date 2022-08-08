# C-Sharp-8.0
Feature of C# 8.0

# Index type 

```
string[] numbers = { "One", "Two", "Three", "Four", "Five", "Six", "Seven", "Eight", "Nine", "Ten"};

Console.WriteLine("---------- Index type -----------");

Console.WriteLine($"Array length # {numbers.Length}");  // 10
Console.WriteLine($"Array.length - N # {numbers.Length - 2}"); // 8

// ^2 == result.Length - N where N is 2 (^2)  10 - 2 = 8 i.e. numbers[8] = "Nine"
Console.WriteLine($"Result of Index# { numbers[^2]}"); // Nine
```

#### Output

```
Nine
```

# Range Type
