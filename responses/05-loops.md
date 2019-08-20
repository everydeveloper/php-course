# Building Loops

## Types of Loops
There are three primary types of loops that we use in PHP.  For this example we will be using the foreach loop.

 - **For**: Set a value and repeat until that value is less than another
 - **While**: Continue looping until something changes
 - **Foreach**: Keep looping for every item in an array

## Build your Loop
Using the $products array we built above, loop through every item making sure to capture the "Key" and the "Value" for that item.  Then display each item and its value on the page on a new line by combining PHP and HTML `<br />` (break) tags.
```php
    foreach($products as $key => $value){
	    echo “The “.$key.” costs “.$value;
    }
```

When you are finished with this section, push your file to github:
```
git add index.php
git commit -m"add foreach loop"
git push origin master
```