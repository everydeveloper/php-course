# Creating Variables

## Building Variables
Variables are an essential part of any project. They hold data that can be modified or used later in a program.

- We define variables in PHP with a $ sign and then we need to decide what the datatype for the variable will be.  For a string of text make sure to put the text in quotes.  If the value is a decimal or integer, no quotes are needed.
- For Example:
```php
$name = "PHP Store";
$customer_number = 1000;
``` 

## Combining text and Variables
Using a period (.), we can concatenate text and variables.  Replace the text in the php tag with the following:
```php
echo "<h1>Welcome to ".$name."!</h1>";
echo "<h2>You are customer number:".$customer_number.".</h2>";
```

Your code should look like this now:

```php
<!DOCTYPE html>
<html>
  <head>
    <title>PHP Store</title>
  </head>
  <body>
    <?php
	    $name = "PHP Store";
			$customer_number = 1000; 
	    echo "<h1>Welcome to ".$name."!</h1>";
	    echo "<h2>You are customer number:".$customer_number.".</h2>";
    ?>
  </body>
</html>
```

Refresh your browser and you should these sentences: _Welcome to PHP Store! You are customer number:1000._

If that worked, push your file to GitHub for the next step:
```
git add index.php
git commit -m"add variables"
git push origin master
```