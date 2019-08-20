# Conditional Statements

## Understanding "if"

If statements are one of the most critical procedures in php decision making since it helps your program know what and when to output based on pre-set conditions.

 - The "if" statement is as simple as "if a condition exists, then do something otherwise (else) do something else".
 - Each statement is made up of 4 sections

 1. The if which starts the statement
 2. The condition encapsulated by parentheses ( )
 3. The body encapsulated by brackets { }
 4. The else which is optional

## Build your "if" statement

Inside of the loop we just created, we want to build an if statement that checks to see if the `$key` is the same value as the `$selected_product` variable.  We do this by using double equal signs (`==`).  This is the condition.
```php
    if($key == $selected_product){
    	echo $key; // nothing should output here except "Computer"
    }
```

When you are finished with this section, push your file to github for the next step:
```
git add index.php
git commit -m"add conditional statement"
git push origin master
```