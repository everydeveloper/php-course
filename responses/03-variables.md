# Creating Variables

## Building Variables
Variables are an essential part of any project. They hold data that can be modified or used later in a program.

 - We define variables in PHP with a $ sign and then we need to decide what the datatype for the variable will be.  For a string of text make sure to put the text in quotes.  If the value is a decimal or integer, no quotes are needed.
 - Build the following variables inside of your PHP tags we built earlier:
```php
$tax_value = .0825; // This is the tax value

$selected_product = “Computer”; // This is the product we are looking for
``` 

## Combining text and Variables
Using a period (.), we can concatenate text and variables.  Replace the word "Computer" and its value with the corresponding variables that we built above.
```php
echo "<h1> The ".$selected_product." is $".$value." after tax. </h1>";
```
When you are finished with this section, push your file to github for the next step:
```
git add index.php
git commit -m"add variables"
git push origin master
```