## Building variables with an Array
Arrays are groupings of information that can be tied to a variable.  Arrays have keys and keys have values.  For example: 
```php
  $ArrayVariable['keyName'] = 'something';
```
Build an array for a series of products and their prices under the variables we created in the previous step.
```php
  $products['Computer']=750;
  $products['Car']=15000;
  $products['iPhone']=1000;
  $products['Toaster']=75;
```
You can access the value stored in an array like this:
```php
echo "<p>A car costs ".$products['Car']."</p>";
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
      $credit = 1000; 

      echo "<h1>Welcome to ".$name."!</h1>";
      echo "<h2>You have $".$credit." in your wallet.</h2>";

	    $products['Computer']=750;
	    $products['Car']=15000;
	    $products['iPhone']=1000;
	    $products['Toaster']=75;

	    echo "<p>A car costs $".$products['Car']."</p>";
    ?>
  </body>
</html>
```

Save your file and refresh your browser. You should see a new sentence on your web page.

Copy and paste the new sentence as a comment on this issue for the next step.
