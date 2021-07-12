**Array**

* Arrays are ordered sequence of data
* They can contain different datatype
* Unlike strings, negative numbers cannot be used to access data


```php
<?php

  $programmingLanguages = ["PHP", "Go", "Javascript", "Python"];
  
  echo $programmingLanguages[1];  // Go

?>
```

<br><br>

Associative Array
* If keys for arrays are defined, they are called Associative array
* Keys can only be string and integer
* If they arent defined, numeric keys from 0 are assumed
 

```php
<?php

  $employee = ["name" => "John Smith", "age" => 35, "occupation" => "Software Engineer" ];
  echo $programmingLanguages["age"];  // 35
  
  $letters = ['a', 'b', 'c', 50 => 'd', 'e', 'f'];
  print_r($letters);  // 0 => 'a', 1 => 'b', 2 => 'c', 50 => 'd', 51 => 'e', 52 => 'f' 
  

?>
```

<br><br>

Array Functions
* Difference between `array_key_exists` and `isset` is that `isset` will return true if key exist and value is not null 
but `array_key_exists` will return true even if the value is null

```php
<?php

  $programmingLanguages = ["PHP", "Go", "Javascript", "Python"];
  
  // Size of array
  echo count($programmingLanguages);  // 4
  
  // Add element at the end
  $programmingLanguages[] = "C++";
  array_push($programmingLanguages, "Typescript");
  array_push($programmingLanguages, "C", "Ruby");
  
  // Remove element from the end
  array_pop($programmingLanguages);  // Ruby
  
  // Remove element from the start
  array_shift($programmingLanguages);  // PHP
  
  // Check if key exists in array
  $employee = ["name" => "John Smith", "age" => 35, "occupation" => "Software Engineer" ];
  array_key_exists("occupation", $employee);  // true
  
?>
```

<br><br>

Casting

```php
<?php
  
  $x = (array) 5;
  echo $x;  // [5]
  

?>
```

<br><br>
