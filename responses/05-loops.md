You just made your first php array!

Arrays are a better way to store complex data than regular variables. Next, we will learn about loops, which are used to repeat a set of instructions until a condition is met. 

# Building Loops

## Types of Loops
There are three primary types of loops that we use in PHP.  For this example we will be using the foreach loop.

 - **For**: Set a value and repeat until that value is less than another
 - **While**: Continue looping until something changes
 - **Foreach**: Keep looping for every item in an array

## Looping through our array
Let's use a foreach loop to display every key and value in our $products array as 'p' tags. This is much more efficient than listing each manually (imagine if there were thousands of products!)

Add this loop after your array values:
```php
    foreach($products as $key => $value){
	    echo "<p>The ".$key." costs ".$value"</p>";
    }
```

You code should look like this now:

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

	    foreach($products as $key => $value){
		    echo "<p>The ".$key." costs ".$value."</p>";
	    }

    ?>
  </body>
</html>

```

If it worked, you should see a list of products and their values. When you are finished with this section, push your file to github:
```
git add index.php
git commit -m"add foreach loop"
git push origin master
```