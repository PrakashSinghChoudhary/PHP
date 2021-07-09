**Data Types**

* PHP is dynamically typed (or also known as weakly typed language) where the type of the variable is not required to be defined  
* Also the type of the variable can change after it has been defined
* Dynamically typed languages check type at runtime while statically typed languages mean the type checking happens at compile time
* Dynamically typed languages are more flexible but that flexible comes at the price of performance and can lead to unexpected bugs

<br>

Scalar Types
* bool
* int
* float
* string

Compound Types
* array
* object
* callable
* iterable

Special Types
* resources
* null

<br><br>

Get type of a variable
```php
<?php

  $isActive = true;
  echo gettype($isActive);  // boolean
  
?>
```
<br><br>

Type hinting  
* Type hinting will try to convert a value to type defined in function. It the type cannot be converted then PHP will throw an error
* PHP will convert the type but the type can be changed again inside the function 

```php
<?php

  function sum($x, $y) {
    var_dump($x, $y);  // int(2) string(1) "3"
    return $x + $y;
  }
  echo sum(2, "3");  // 5
  
  
  function sum(int $x, int $y) {
    var_dump($x, $y);  // int(2) int(3)
    return $x + $y;
  }
  echo sum(2, "3");  // 5

  
  function sum(int $x, int $y) {
    var_dump($x, $y);  // int(2) int(3)
    return $x + $y;
  }
  echo sum(2.5, "3");  // 5
  
?>
```

<br><br>

Enable strict mode in PHP  
* Strict mode will help in avoiding/reducing bugs
* It will throw an error if incorrect type is passed to a function
* Strict mode will not throw an error if the type is defined as float and int value is passed

```php
<?php
  
  declare(strict_types=1);
  
  // ...code
  
?>
```

<br><br>

Type casing  

```php
<?php
  
  $x = "5";
  var_dump($x);  // string(1) "5"
  
  
  $x = (int) "5";
  var_dump($x);  // int(5)
  
?>
```

