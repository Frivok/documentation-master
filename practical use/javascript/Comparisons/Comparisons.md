# Comparisons

- [Comparisons](#comparisons)
- [JavaScript Comparison and Logical Operators](#javascript-comparison-and-logical-operators)
- [Comparison Operators](#comparison-operators)
- [How Can it be Used](#how-can-it-be-used)
- [Logical Operators](#logical-operators)
- [Conditional (Ternary) Operator](#conditional-ternary-operator)
- [Comparing Different Types](#comparing-different-types)

# JavaScript Comparison and Logical Operators

```bash
Comparison and Logical operators are used to test for true or false.
```

# Comparison Operators

```bash
Comparison operators are used in logical statements to determine equality or difference between variables or values.

Given that x = 5, the table below explains the comparison operators:

Operator 	         Description 	        Comparing     	Returns

== 	                 equal to 	            x == 8 	        false 	
                                            x  == 5 	    true 	
                                            x == "5" 	    true 

===                 equal value 
                    and equal type          x === 5 	    true 	
                                            x === "5" 	    false 

!= 	                not equal 	            x != 8 	        true

!== 	            not equal value
                    or not equal type       x !== 5 	    false 	
                                            x !== "5" 	    true 	
                                            x !== 8 	    true 	

>                   greater than 	        x > 8 	        false 	

< 	                less than 	            x < 8 	        true 	

>= 	                greater than or 
                    equal to 	            x >= 8 	        false

<= 	                less than or 
                    equal to 	            x <= 8 	        true
```

# How Can it be Used

```bash
Comparison operators can be used in conditional statements to compare values and take action depending on the result:

if (age < 18) text = "Too young";
```

# Logical Operators

```bash
Logical operators are used to determine the logic between variables or values.

Given that x = 6 and y = 3, the table below explains the logical operators:
Operator 	Description 	Example 	Try it
&& 	and 	(x < 10 && y > 1) is true 	
|| 	or 	(x == 5 || y == 5) is false 	
! 	not 	!(x == y) is true 	
```

# Conditional (Ternary) Operator

```bash
JavaScript also contains a conditional operator that assigns a value to a variable based on some condition.

Syntax

variablename = (condition) ? value1:value2 

Example

var voteable = (age < 18) ? "Too young":"Old enough";

If the variable age is a value below 18, the value of the variable voteable will be "Too young", otherwise the value of voteable will be "Old enough".
```

# Comparing Different Types

```bash
Comparing data of different types may give unexpected results.

When comparing a string with a number, JavaScript will convert the string to a number when doing the comparison. An empty string converts to 0. A non-numeric string converts to NaN which is always false.

Case               Value
2 < 12             true
2 < "12"           true
2 < "John" 	       false 	
2 > "John" 	       false 	
2 == "John" 	   false 	
"2" < "12" 	       false 	
"2" > "12"         true 	
"2" == "12" 	   false 	

When comparing two strings, "2" will be greater than "12", because (alphabetically) 1 is less than 2.

To secure a proper result, variables should be converted to the proper type before comparison:

age = Number(age);
if (isNaN(age)) {
  voteable = "Input is not a number";
} else {
  voteable = (age < 18) ? "Too young" : "Old enough";
}
```