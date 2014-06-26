phpserial
=========

PHP Serial Key Generator, very simple but effective. Includes random keys, multipart random keys and custom formatted keys. 

Simple and easy.

```php
<?

require_once('/path/to/src/php-serial.class.php');

// Random key with length of 10
var_dump( Serial::random(10) ); // String(10) "5KGH89FSE4"

// We can generate keys defining the number of parts, length 
// of each part and seperating character parameters
var_dump( Serial::newSerial(4, 5, '-') ); // String(23) "UWB46-8SEER-6A46W-HADP8"

//Custom formatted keys can also be generated, using `*` to donate where to replace the characters
var_dump( Serial::costumSerial('H*E*L*L*O*W*O*R*L*D') ); // String(19) "HFEIL5LSO9WPO2RSLCD"

?>
