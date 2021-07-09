**Booleans**

* Boolean is a simple representation of a truth value
* It can be either be `true` or `false`
* Echo will print `1` for true and `""` for false
* `true` and `false` are predefined constants that can be either lowercase, uppercase or mixedcase
* They are mostly used within a control structure

```php
<?php
  
  $isComplete = true;
  
?>
```

<br><br>

Convertion
* If evaluated, non boolean values are converted to boolean on the fly 
* integers 0, -0 = false
* floats 0.0, -0.0 = false
* string "", "0" = false
* array [] = false
* null = false

<br><br>

Check if a value is boolean

```php
<?php
  
  $isComplete = true;
  is_bool($isComplete);
  
?>
```
