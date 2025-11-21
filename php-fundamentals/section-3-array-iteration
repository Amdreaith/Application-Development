## **Section 3: PHP Array and Iteration**

### **I. PHP Intro to Array**
*   An array is a special variable that can hold **more than one value** under a single name.
*   Values are stored in **key-value pairs**.
*   Created with the `array()` construct or the short array syntax `[]`.

**Indexed Array (Default numeric keys):**
```php
$fruits = array("Apple", "Banana", "Orange");
// or
$fruits = ["Apple", "Banana", "Orange"];
```

---

### **II. PHP Array Functions**
*   `count($array)` - Count the number of elements.
*   `array_push($array, $value)` - Add to the end of the array.
*   `array_pop($array)` - Remove from the end.
*   `array_unshift($array, $value)` - Add to the beginning.
*   `array_shift($array)` - Remove from the beginning.
*   `in_array($value, $array)` - Check if a value exists.
*   `array_merge($array1, $array2)` - Merge two or more arrays.
*   `sort($array)`, `rsort($array)` - Sort ascending/descending (by value).
*   `array_reverse($array)` - Return a new array with elements in reverse order.

---

### **III. PHP Associative Array**
*   An array where each key is a **custom string** instead of a number.
*   Key-value pairs are defined using the `=>` operator.

```php
$person = [
    "name" => "John",
    "age" => 30,
    "city" => "New York"
];
// Access value by its key:
echo $person["name"]; // Outputs: John
```



### **IV. PHP Multi-Dimensional Array**
*   An array that contains **one or more arrays** as its values.
*   Useful for storing complex, tabular data.

```php
$users = [
    ["Alice", "alice@email.com", 25],
    ["Bob", "bob@email.com", 30],
    ["Charlie", "charlie@email.com", 35]
];
// Access value:
echo $users[1][0]; // Outputs: Bob (First element of the second array)
```



### **V. PHP Basic Loops**
**1. `while` Loop**
*   Repeats a block of code as long as the condition is true.
```php
$i = 1;
while ($i <= 5) {
    echo $i;
    $i++;
}
```

**2. `do...while` Loop**
*   Executes the code block once, *then* repeats while the condition is true.
```php
$i = 1;
do {
    echo $i;
    $i++;
} while ($i <= 5);
```

**3. `for` Loop**
*   Used when the number of iterations is known.
```php
for ($i = 0; $i < 5; $i++) {
    echo "Number: $i";
}
```


### **VI. PHP Nested Loops**
*   A loop inside another loop.

```php
// Example: Creating a multiplication table
for ($i = 1; $i <= 3; $i++) {
    for ($j = 1; $j <= 3; $j++) {
        echo $i * $j . " ";
    }
    echo "<br>";
}
```


### **VII. PHP Looping through Array**
**`foreach` Loop (Best for arrays)**
*   The simplest way to iterate over arrays.

**For Indexed Arrays:**
```php
$colors = ["Red", "Green", "Blue"];
foreach ($colors as $color) {
    echo $color;
}
```

**For Associative Arrays:**
```php
$person = ["name" => "John", "age" => 30];
foreach ($person as $key => $value) {
    echo "$key: $value";
}
```


### **VIII. PHP Multi-Dimensional Array Iteration**
*   Use **nested `foreach` loops** to access all elements.

```php
$users = [
    ["name" => "Alice", "email" => "alice@email.com"],
    ["name" => "Bob", "email" => "bob@email.com"]
];

foreach ($users as $user) {
    // $user is now an associative array
    echo "Name: " . $user["name"];
    echo "Email: " . $user["email"];
}
```

**For a complex multi-dimensional array:**
```php
$matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

foreach ($matrix as $row) {
    foreach ($row as $cell) {
        echo $cell . " ";
    }
    echo "<br>";
}
```