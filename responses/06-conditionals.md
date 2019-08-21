# Conditional Statements

"If" statements are one of the most critical procedures in php decision making. They give you control over what is displayed, making the display more dynamic.

An "if" statement tests if a condition is true or false. If true, it will run the code following it. If false, it will skip that code and optionally run code in an "else" statement.

## Build your "if" statement

We can use an "if" statement to display products we can afford. Let's make another foreach loop, but this time test if the value is less than or equal our credit variable.

Add the following to the end of your php tag:

```php
echo "<h2>Items you can afford</h2>";

foreach($products as $key => $value){
  if($value <= $credit ){
  	echo "<p>".$key."</p>"; 
  }
```

Refresh your page, and make sure these products are listed: "Computer, iPhone, and Toaster".

Your code should look like this:

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

	    echo "<h2>Items you can afford</h2>";

	    foreach($products as $key => $value){
		    if($value <= $credit ){
		    	echo "<p>".$key."</p>"; 
		    }
	    }
    ?>
  </body>
</html>
```

When you are finished with this section, push your file to GitHub for the next step:

```
git add index.php
git commit -m"add conditional statement"
git push origin master
```