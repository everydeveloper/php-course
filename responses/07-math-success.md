Alright, 66 was the right answer! Now lets write a function that will calculate tax for our products.

## Using Default Functions

There are many pre-built default functions available with php, so you should check to see if one exists before trying to create one. For instance, if we want to round 811.882 to 811.88 we can use the round() function which requires a variable and the number of digits to round to.
For example:
```php
round(811.882,2); // should return 811.88
```
## Create a Function

At the very bottom of the PHP code (but before the `?>`), type the following code to create a tax calculating function:
```php
  function tax_calc($amount,$tax){
  	$calculate_tax = $amount*$tax;
  	$amount = round($amount+$calculate_tax,2);
  	return $amount;
  }
```
When when want to use this function, pass in values for $amount and $tax like so:
```php
echo tax_calc(750,0.223); // When you refresh your page you should the value 917.25 at the bottom of the screen.
```
When you have successfully defined and called your function, push your changes to GitHub.
```
git add index.php
git commit -m"add tax calc function"
git push origin master
```
