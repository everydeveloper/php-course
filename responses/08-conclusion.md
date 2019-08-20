# Conclusion

At this point we just need to add all the pieces together and we will have a functioning program that searches a php array for the key of “Computer” and uses that value to calculate tax and display it on the screen.
```php
<!DOCTYPE html>
<html>
  <head>
    <title>This is a title</title>
  </head>
  <body>
<?php
$tax_value = .0825;
$selected_product = "Computer";

//Build an array of products
$products['Computer']=750;
$products['Car']=15000;
$products['iPhone']=1000;
$products['Toaster']=75;

foreach($products as $key => $value){
	if($key==$selected_product){
		$value = tax_calc($value,$tax_value) ;
		echo "<h1> The ".$selected_product." is ".$value." after tax. </h1>";
	}
}

function tax_calc($amount,$tax){
	$calculate_tax = $amount*$tax;
	$amount = round($amount+$calculate_tax,2);
	$addDollar_in_front = "$".$amount;
	return $addDollar_in_front;
}
?>
  </body>
</html>
```

Check to make sure your code looks like the above. **Close this issue when you are finished**