# Setting up PHP

PHP is server-side code that runs on top of a normal HTML website.  This means you can use HTML and PHP together.

 - Get started by creating a PHP document in the www folder in WAMP.  Index.php is considered by most websites to be the "home page"
 - Open index.php in your text editor and type the following HTML code
```php
<!DOCTYPE html>
<html>
  <head>
    <title>PHP Store</title>
  </head>
  <body>
    <?php
    // Using two forward slashes we create comments in php.
    // Within the php tag, we can insert values into our HTML.
    echo "<h1>Welcome!</h1>";
    ?>
  </body>
</html>
```

# Displaying Content
In this example, we used the "echo" command to insert an HTML header within the php tags. All of our php code will be contained in these tags. 

**Make sure you always end every statement with a semicolon**

In your browser, click on the php-course folder, and you should see the header we inserted being displayed.

If it worked, save your changes to GitHub. 
```
git add index.php
git commit -m"initial php setup"
git push origin master
```