**Floats**

* Floating points are the numbers with a decimal point
* They can also be expressed in expotential form
* Its minimum and maximum size depends on the platform and can be checked using predefined constants like `PHP_FLOAT_MIN`, `PHP_FLOAT_MAX`
* If the float is defined with a out of bound value, it will be converted to `INF` (short for Infinity)



```php
<?php

  $x = 13.5;
  echo $x;  // 13.5
  
  $y = 13.5e3
  echo $y  // 13500
  
  $z = 13.5e-3
  echo $z  // 0.0135

?>
```

<br><br>

Casting

For casting, float can be used 
```php
<?php
  
  $x = (float) 5;  // 5
  $x = (float) "8.7awwdfsfa";  // 8.7
  $x = (float) "test";  // 0
  
?>
```
