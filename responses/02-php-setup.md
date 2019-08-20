# Formatting and Structure
## Setting up PHP

PHP is server-side code that runs on top of a normal HTML website.  This means you can use HTML and PHP together.

 - Get started by creating a PHP document in the www folder in WAMP.  Index.php is considered by most websites to be the "home page"
 - Open index.php in notepad++ and type the following HTML code
```php
<!DOCTYPE html>
<html>
  <head>
    <title>This is a title</title>
  </head>
  <body>
    <?php
    // Using two forward slashes we create comments in php
    ?>
  </body>
</html>
```

## Displaying Content
Next, use the "echo" command to display text on the page. We will include html Header 1(`<h1></h1>`) tags in this example.
<![endif]-->

```php
echo "<h1> The Computer is $750 </h1>";
```
**Make sure you Always end every statement with a semicolon**

When you are finished with this section, push your file to github for the next step:
```
git add index.php
git commit -m"initial php setup"
git push origin master
```