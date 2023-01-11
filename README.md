# slips 

```
<?php
$celsius = 17 ;
$fahrenheit = (($celsius*9)/5)+32 ;
echo("Temperature in Fahrenheit is: ");
?>

Q2

<html>
<head>
<title>Book price service</title>
</head>
<body>
<form method="post" action="book_price_service.php" style="margin:
auto; text-align: center; margin-top: 100px; font-size:
larger; font-family: 'Lucida Sans'">
Enter book name: <input type="text" name="book_name"></br></br>
<input type="submit" value="Get price">
</form>
</body>
</html>


<html>
<head>
<title>Book price service</title>
</head>
<body style="margin:
auto; text-align: center; margin-top: 100px; font-size:
larger; font-family: 'Lucida Sans', 'Lucida Sans Regular',
'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana,
sans-serif;">
<?php
function getBookPrice($name) {
$prices = array(
"The Great Gatsby" => 19.99,
"To Kill a Mockingbird" => 14.99,
"Pride and Prejudice" => 12.99,
"The Catcher in the Rye" => 9.99
);
return isset($prices[$name]) ? $prices[$name] : "Book not found";
}
$book_name = $_POST['book_name'];
$book_price = getBookPrice($book_name);
echo "Book name: $book_name"."<br><br>"."Book price: $book_price";
?>
</body>
</html>
```
