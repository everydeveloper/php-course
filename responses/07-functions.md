# Functions

Functions are pre-built commands in PHP that do some of the hard work for you.  You can also write your own custom function. The function we will write will calculate tax, but first let's go over using math in PHP



## Using Math

By using math symbols you can add, subtract, multiply or divide variables. Add this the bottom of your php tags
```php
	$amount=800;
	$taxRate=0.0825
  $addedTax= $amount*$taxRate;  //amount = 800, tax = .0825
```

## Calling an Existing Function

There are many functions available to call, so you should check to see if one exists before trying to create one.  In this case we want to round 811.882 to 811.88 and we will use the round() function which requires a variable and the number of digits to round to.
```php
    $amount = round($amount+calculate_tax,2); // the amount, add tax and round
```
## Create a Function

At the very bottom of the page, type the following code to create your function:
```php
    function tax_calc($amount,$tax){
    	$calculate_tax = $amount*$tax;
    	$amount = round($amount+$calculate_tax,2);
    	$addDollar_in_front = "$".$amount;
    	return $addDollar_in_front;
    }
```

Whne you have added this function to your code, push your changes to github.
```
git add index.php
git commit -m"add tax calc function"
git push origin master
```