# C-Sharp-8.0
Feature of C# 8.0

# Index type 

| 0       | 1    | 2       | 3    | 4       | 5    | 6       | 7    | 8       | 9    |
|---------|------|---------|------|---------|------|---------|------|---------|------|
| One     | Two  | Three   |Four  |Five     |Six   |Seven    |Eight |Nine     |Ten   |  


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

Example 1#

| 0       | 1    | 2       | 3    | 4       | 5    | 6       | 7    | 8       | 9    |
|---------|------|---------|------|---------|------|---------|------|---------|------|
| One     | Two  | Three   |Four  |Five     |Six   |Seven    |Eight |Nine     |Ten   |  

```
string[] numbers = { "One", "Two", "Three", "Four", "Five", "Six", "Seven", "Eight", "Nine", "Ten" };

var result = numbers[2..4]; // Three, Four

foreach (var s in result)  // Three, Four
{
    Console.WriteLine(s);
}
```

```
Output:
Three, Four
```

Example 2#

| 0       | 1    | 2       | 3    | 4       | 5    | 6       | 7    | 8       | 9    |
|---------|------|---------|------|---------|------|---------|------|---------|------|
| One     | Two  | Three   |Four  |Five     |Six   |Seven    |Eight |Nine     |Ten   |  

```
string[] numbers = { "One", "Two", "Three", "Four", "Five", "Six", "Seven", "Eight", "Nine", "Ten"};

Range range = 1..4;

var result1 = numbers[range];

foreach (var v1 in result1) // Two, Three, Four
{
     Console.WriteLine(v1);
}
```

```
Output:
Two, Three, Four
```

Example 3#

```
foreach (var v1 in numbers[2..]) 
Console.WriteLine(v1);
```
```
Output:
"Three", "Four", "Five", "Six", "Seven", "Eight", "Nine", "Ten" 
```

```
foreach (var v1 in numbers[..4]) 
Console.WriteLine(v1); 
```
```
Output:
"One", "Two", "Three", "Four"
```

```
foreach (var v1 in numbers[..]) 
Console.WriteLine(v1); 
```

```
Output:
"One", "Two", "Three", "Four", "Five", "Six", "Seven", "Eight", "Nine", "Ten"
```

```
foreach (var v1 in numbers[2..4]) 
Console.WriteLine(v1);

Output:
"Three", "Four"
```

```
int i = 2;
Range range1 = i..(i+2);
foreach (var v1 in numbers[range1]) 
Console.WriteLine(v1);

Output:
"Three", "Four"
```


