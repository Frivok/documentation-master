# C#

- [C](#c)
  - [Commands](#commands)
    - [String (contains a word)](#string-contains-a-word)
    - [Int (contains a number)](#int-contains-a-number)
    - [Var (same as int and string, cannot be a constant)](#var-same-as-int-and-string-cannot-be-a-constant)
    - [Float (contains a decimal number like 1.5)](#float-contains-a-decimal-number-like-15)
    - [Double (same as float but with a higher number limit)](#double-same-as-float-but-with-a-higher-number-limit)
    - [Decimal (same as double but with a higher number limit)](#decimal-same-as-double-but-with-a-higher-number-limit)
    - [If (an action always true and what happens after its true)](#if-an-action-always-true-and-what-happens-after-its-true)
    - [If-Else (same as if but with else in case if isn't accomplished)](#if-else-same-as-if-but-with-else-in-case-if-isnt-accomplished)
    - [Switch (equivalent to if-else utilised if there is more than 3 conditions)](#switch-equivalent-to-if-else-utilised-if-there-is-more-than-3-conditions)
    - [Void (used as a type of return for a method so it doesn't return a value)](#void-used-as-a-type-of-return-for-a-method-so-it-doesnt-return-a-value)

## Commands

[C#](https://docs.microsoft.com/fr-fr/dotnet/csharp/programming-guide/)

### String (contains a word)

```bash
string
```

### Int (contains a number)

```bash
int
```

### Var (same as int and string, cannot be a constant)

```bash
var
```

### Float (contains a decimal number like 1.5)

```bash
float
```

### Double (same as float but with a higher number limit)

```bash
double
```

### Decimal (same as double but with a higher number limit)

```bash
decimal
```

### If (an action always true and what happens after its true)

```bash
if ("action")
{
  "then statement(what happens after action)"
}
```

### If-Else (same as if but with else in case if isn't accomplished)

```bash
if ("action")
{
  "then statement, if it doesn't work uses else"
}
else
{
   "else statement, what happens if if doesn't work";
}
```

### Switch (equivalent to if-else utilised if there is more than 3 conditions)

```bash
example day =3

switch("expression","aka day")
{
  case 0
  "stuff ex:" Console.WriteLine(Monday);
  break;
  case 1
  "stuff if case 0 doesn't work ex:" Console.WriteLine(Tuesday);
  break;
  case 2
  "stuff if case 1 doesn't work ex:" Console.WriteLine(Wednesday)
  break;
}
```

### Void (used as a type of return for a method so it doesn't return a value)

```bash
public static void Example(){

}
```
