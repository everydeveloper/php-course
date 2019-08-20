## Building variables with an Array
Arrays are groupings of information that can be tied to a variable.  Arrays have keys and keys have values.  For example: 
```php
  $ArrayVariable["keyName"] = "something";
```
Build an array for a series of products and their prices under the variables we just created above.
```php
    $products['Computer']=750;
    $products['Car']=15000;
    $products['iPhone']=1000;
    $products['Toaster']=75;
```
When you are finished with this section, push your file to github for the next step:
```
git add index.php
git commit -m"add array"
git push origin master
```