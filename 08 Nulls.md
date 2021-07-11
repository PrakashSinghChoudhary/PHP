**Null**

* Nulls are special datatype that represents a variable with no value
* A variable can be `NULL` if it is assigned a constanst `NULL`, or if its not defined yet or it has be unset
* `is_null` function can be used to determine if a variable is `NULL` or not

```php
<?php

  $x = null;
  
  $y = 5;
  unset($y);
  
  echo $x;  // NULL
  echo $y;  // NULL
  echo $z;  // NULL
  
?>
```

<br><br>

Casting of null to other datatypes

```php
<?php

  $x = null;
  
  echo (string) $x;    // ""
  echo (integer) $x;   // 0
  echo (bool) $x;      // false
  echo (array) $x;     // []
  
?>
```

<br><br>

