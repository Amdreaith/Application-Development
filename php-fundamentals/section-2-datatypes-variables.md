## Section 2: PHP Data types, Variables and Built in functions

Project Setup (Laragon)
Path: C:\laragon\www\
    ---> go to C:Drive and select "laragon" >>> folder "www" >>> then create a folder.

### I. PHP Tags Printing and Comments

<?php // Opening tag for PHP code ?>

##### Printing/Output:

echo "Hello World"; // Outputs one or more strings.

print "Hello"; // Outputs a single string (returns 1, slower than echo).

var_dump($variable); // Displays structured info (type and value), great for debugging.

print_r($array); // Displays human-readable info, best for arrays.

##### Comments:

// Single-line comment

# Also a single-line comment

/* Multi-line comment */



### II. PHP Variables
>> starts with a "$"  //example: $name
>> must start with a letter or underscore
>> names are case sensitive
>> No need to declare type; it's determined at runtime.

### III. PHP Data Types

##### Scalar Types (single value):

String - Sequence of characters ("Hello")
Integer - Whole number (-5, 0, 100)
Float - Decimal number (3.14, -10.5)
Boolean - true or false

###### Compound Types:

Array - Ordered map (["apple", "banana"])
Object - Instance of a class
NULL - Variable with no value ($x = null;)

### IV. PHP String Concatenation
>> Use "dot(.)" operator to join strings.

![alt text](image-1.png)

### V. PHP Type Casting
>> Manually convert a value from one type to another.

![alt text](image-2.png)

### VI. PHP Arithmetic and Math Functions

Basic Operators: +, -, *, /, % (modulus), ** (exponentiation)

###### Common Math Functions:

abs(-5) // 5 (Absolute value)
round(3.7) // 4
ceil(3.3) // 4 (Round up)
floor(3.9) // 3 (Round down)
rand(1, 10) // Random number between 1 and 10
min(5, 10, 2) // 2
max(5, 10, 2) // 10

### VII. PHP String Functions

strlen($string) //Get string length.

strtoupper($string), strtolower($string) //Change case.

ucfirst($string) //Capitalize first letter.

trim($string) //Remove whitespace from both ends.

substr($string, start, length) //Return part of a string.

str_replace(find, replace, $string) //Replace all occurrences.

strpos($string, search) //Find position of first occurrence.

explode(delimiter, $string) ///Split string into an array.

implode(glue, $array) //Join array elements into a string.


### VIII. PHP Date Function

date(format, timestamp) //Format a local date/time.

time() //Returns current Unix timestamp.



#### note:

Y - Four-digit year

m - Month (01-12)

d - Day (01-31)

H - Hour (00-23)

i - Minutes (00-59)

s - Seconds (00-59)


example :

![alt text](image-3.png)