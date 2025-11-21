## **Section 4: PHP Control Structures and Conditionals**

### **I. The IF Statement**
*   Executes code if a condition is true.

**Basic Syntax:**
```php
if (condition) {
    // code to execute if condition is true
}
```

**if...else:**
```php
if (condition) {
    // code if true
} else {
    // code if false
}
```

**if...elseif...else:**
```php
if (condition1) {
    // code if condition1 is true
} elseif (condition2) {
    // code if condition2 is true
} else {
    // code if all conditions are false
}
```



### **II. Conditional HTML Output**
*   Mix PHP conditionals with HTML for dynamic content.

**Method 1: PHP Tags in HTML**
```php
<div class="message">
    <?php if ($isLoggedIn): ?>
        <p>Welcome back, User!</p>
    <?php else: ?>
        <p>Please log in.</p>
    <?php endif; ?>
</div>
```

**Method 2: Echo/Print in PHP**
```php
<?php
if ($score >= 50) {
    echo "<p class='pass'>You passed!</p>";
} else {
    echo "<p class='fail'>You failed.</p>";
}
?>
```



### **III. Comparison and Logical Operators**

**Comparison Operators:**
*   `==` Equal (value)
*   `===` Identical (value and type)
*   `!=` or `<>` Not equal
*   `!==` Not identical
*   `>` Greater than
*   `<` Less than
*   `>=` Greater than or equal to
*   `<=` Less than or equal to

**Logical Operators:**
*   `&&` or `and` - AND
*   `||` or `or` - OR
*   `!` - NOT
*   `xor` - Exclusive OR (true if either is true, but not both)

```php
if ($age >= 18 && $hasID) {
    echo "You can enter.";
}

if ($role === "admin" || $role === "moderator") {
    echo "Access granted.";
}
```



### **IV. Conditional in Loop**
*   Use conditionals inside loops to control iteration behavior.

```php
// Skip even numbers
for ($i = 1; $i <= 10; $i++) {
    if ($i % 2 == 0) {
        continue; // Skip this iteration
    }
    echo $i . " "; // Output: 1 3 5 7 9
}

// Stop loop when condition met
$numbers = [1, 3, 5, 8, 10];
foreach ($numbers as $num) {
    if ($num > 7) {
        break; // Exit loop entirely
    }
    echo $num . " "; // Output: 1 3 5
}
```



### **V. Switch Case Statement**
*   Alternative to multiple elseif statements for comparing same variable/expression.

```php
$day = "Monday";

switch ($day) {
    case "Monday":
        echo "Start of work week";
        break;
    case "Friday":
        echo "Thank God it's Friday!";
        break;
    case "Saturday":
    case "Sunday":
        echo "Weekend!";
        break;
    default:
        echo "Regular weekday";
}
```

**Important:** Always include `break` to prevent "fall-through" to next case.



### **VI. Ternary Operator**
*   Shorthand for simple if-else statements.

**Syntax:** `(condition) ? value_if_true : value_if_false`

```php
// Traditional if-else
if ($age >= 18) {
    $status = "Adult";
} else {
    $status = "Minor";
}

// Ternary equivalent
$status = ($age >= 18) ? "Adult" : "Minor";

// Can also be used for quick output
echo ($isActive) ? "Online" : "Offline";
```



### **VII. Null Coalescing Operator**
*   Returns the first operand if it exists and is not NULL; otherwise returns the second operand.

**Syntax:** `$value = $a ?? $b;`

```php
// Without null coalescing
$username = isset($_GET['user']) ? $_GET['user'] : 'guest';

// With null coalescing
$username = $_GET['user'] ?? 'guest';

// Multiple fallbacks (PHP 7+)
$username = $_GET['user'] ?? $_POST['user'] ?? 'guest';
```

**Null Coalescing Assignment Operator (PHP 7.4+):**
```php
// Only assign if $array['key'] is null or doesn't exist
$array['key'] ??= 'default_value';
```

