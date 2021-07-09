**Integer**

* Integers are numbers without any decimal points
* It includes all negative, zero and positive numbers 
* Its minimum and maximum size depends on the platform and can be checked using predefined constants like `PHP_INT_MIN`, `PHP_INT_MAX` and `PHP_INT_SIZE`
* If the int is defined with a out of bound value, it will be converted to float 

<br><br>

Define integers in various number system
```php
<?php
  
  //Decimal
  $x = 10; // 5

  // Hexadecimal
  $x = 0x2A;  // 42

  // Octal
  $x = 055;  // 45
  
  // Binary
  $x = 0b11;  // 3
?>
```

<br><br>

Casting
* For casting, either `int` or `integer` can be used 
* If floating number is casted to int, then it will always round down
```php
<?php
  
  $x = (int) "5";
  $x = (integer) "5";
  
  $x = (int) true;  // 1
  $x = (int) false;  // ""
  $x = (int) 5.98;  // 5
  $x = (int) "5.9";  // 5
  $x = (int) "87";  // 87
  $x = (int) "87awwdfsfa";  // 87
  $x = (int) "test";  // 0
  $x = (int) null;  // 0
  
?>
```

<br><br>

Check if a value is integer

```php
<?php
  
  $x = "42";
  is_int($x);  // true
  is_integer($x);  // true
  
?>
```

<br><br>

Using `_` for improving readability of large numbers
```php
<?php
  
  $x = 20_000_000;
  echo $x;  // 20000000
  
?>
```
