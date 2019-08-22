# Conclusion

At this point we just need to add all the pieces together and we will have a functioning program that displays products with added tax. Your code should look like this now:
```php
<!DOCTYPE html>
<html>
  <head>
    <title>PHP Store</title>
  </head>
  <body>
    <?php
	    $name = "PHP Store";
			$credit = 1000; 

	    echo "<h1>Welcome to ".$name."!</h1>";
	    echo "<h2>You have $".$credit." in your wallet.</h2>";

		  $products['Computer']=750;
	    $products['Car']=15000;
	    $products['iPhone']=1000;
	    $products['Toaster']=75;

      $taxRate=0.0825;

      function tax_calc($amount,$tax){
	    	$addedTax = $amount*$tax;
	    	$amountWithTax = round($amount+$addedTax,2);
	    	return $amountWithTax;
    	}

	    foreach($products as $key => $value){
	    	$costWithTax = tax_calc($value,$taxRate);
		    echo "<p>The ".$key." costs ".$costWithTax." with tax</p>";
	    }

	    echo "<h2>Items you can afford</h2>";

	    foreach($products as $key => $value){
	    	$costWithTax = tax_calc($value,$taxRate);
		    if($costWithTax <= $credit ){
		    	echo "<p>".$key."</p>"; 
		    }
	    }
    ?>
  </body>
</html>
```
... 🤔 
Looks like we can't afford the iPhone after all (after taxes)! 

**Close this issue when you are finished**