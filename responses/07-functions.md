# Functions

Functions are pre-built commands in PHP that do some of the hard work for you. You can also write your own custom function. The function we will write will calculate tax, but first let's go over using math in PHP

## Using Math

By using math symbols you can add(+), subtract(-), multiply(*) or divide(/) variables. Add this to the bottom of your php tags:
```php
$amount=800;
$taxRate=0.0825;
$addedTax= $amount*$taxRate;  //amount = 800, tax = .0825
echo $addedTax
```
Refresh the page, and leave a comment with the value of $addedTax to continue. 

