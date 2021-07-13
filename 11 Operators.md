**Operators**

* An operator is something that takes one or more expressions that results in a value
* If an operator only takes a single value it is called unary operator, if it takes two values it is called binary operator, 
if it requires three values then it is called ternary operator

<br><br>

Arithmetic Operators: (+ - * / % *\*)  

It allows to perform common arithmetic operations like addition, subtraction, multiplication, division, modolus and exponentation.

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
  
  

?>
