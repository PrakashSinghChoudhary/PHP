**Strings**

* String is a sequence of characters
* They can be placed within single `''` or double `""` quotes
* The difference between single and double quote is that variable cannot be used inside single quotes


```php
<?php
  
  $firstName = "Will";
  $lastName = "Smith";
  $fullName = "$firstName $lastName";
  $fullName = "${firstName} ${lastName}";  // Alternate way
  $fullName = "{$firstName} {$lastName}";  // Alternate way
  
  echo $firstName;  // Will
  echo $lastName;  // Smith
  echo $fullName;  // Will Smith
  
?>
```

<br><br>

Access a specific character in string

```php
<?php
  
  $firstName = "Will";
  
  echo $firstName[0];  // W
  echo $firstName[-3];  // i
  
?>
```

<br><br>

Modify a specific character in string

```php
<?php
  
  $firstName = "Will";
  
  echo $firstName[0] = "B";
  echo $firstName;  // Bill
  
?>
```

<br><br>

Heredoc and Nowdoc
* They are ways to handle long and multiline string 
* They may contain both single and double quotes and complex expression without the need to escape them
* Difference is that Heredoc treats strings as double quotes and Nowdoc treats strings as single quotes
* They can also contain HTML tags and it will be parsed
* They also respect spaces and tabs and will display them

```php
<?php
  
  $one = 1;
  
  // Heredoc
  $text = <<<TEXT
    Line $one
    Line 2
    Line 3  
  TEXT;
  
  // Nowdoc
  $text = <<<'TEXT'
    Line $one
    Line 2
    Line 3  
  TEXT;
  
?>
```
