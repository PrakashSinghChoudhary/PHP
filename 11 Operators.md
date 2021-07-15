**Operators**

* An operator is something that takes one or more expressions that results in a value
* If an operator only takes a single value it is called unary operator, if it takes two values it is called binary operator, 
if it requires three values then it is called ternary operator

<br><br>

Arithmetic Operators: (+ - * / % *\*)  

It allows to perform common arithmetic operations like addition, subtraction, multiplication, division, modulus and exponentation

```php
<php

  $x = 10;
  $y = 5;
  
  echo $x + $y;  // 15
  echo $x - $y;  // 5
  echo $x * $y;  // 50
  echo $x / $y;  // 2
  echo $x % $y;  // 0
  echo $x ** $y;  // 100000
  
  // Converts string to int
  $x = +'10';

  // Division also return float unless both of the operands are int and evenly divisible
  echo 10 / 3;  // 3.333333333 
  
  // Modulus always returns 0 by casting both the operands into int, fmod can be used to get a float value
  echo 10.5 % 2.9;  // 0
  echo fmod(10.5, 2.9)  // 1.8000000000000
  
?>
```

<br><br>

Assignment Operators: (= += -= *= /= %= *\*=)  

It allows to assign values to a variable and helps shorten the code for arithmetic operator

```php
<php

  $x = 10;  // Assignment operator
  $x += 5;  // i.e. $x = $x + 5 
  
?>
```

<br><br>

String Operators: (. .=)  

It allows to concat strings and use assignment operator with concatenation

```php
<php

  $firstName = "John";
  $lastName = "Smith";
  
  echo $firstName . ' ' . $lastName;  // John Smith
  $firstName .= ' Smith';
  echo $firstName;  // John Smith
?>
```

<br><br>

Comparison Operators: (= === != <> !== < > <= >= <=> ?? ?:)  

It allows to compare variables with each other

```php
<php

  $x = 5;
  $y = '5';
  
  // Compare value
  echo $x == $y;  // true
  
  // Compare value and type
  echo $x === $y;  // false
  
  // Compare value (same as <>)
  echo $x != $y;  // false
  
  // Compare value and type
  echo $x !== $y;  // true
  
  echo 7 < 3;  // false
  echo 7 > 3;  // true
  
  // Spaceship operator: returns 0 if both operands are equal, return -1 if 1st operand is less than 2nd and return 1 if 1st operand is greater than 2nd
  echo 7 <=> 3;   // 1
  
  // Null Coalescing Operator
  $x = null;
  $y = $x ?? 'hello';
  echo $y;  // hello
  
  // Ternary operator
  $result = $value === 5 ? 'Success': 'Try again';
   
?>
```
