PHP IP Grabber
=======================
Don't be stupid and use this to threaten people i made this for
protection and this can be used for you want you can jack up and fiddle
around with the source code i am not 0.01% responsable if you perform a
stupid act.

- Peter aka dzt aka Virtual God

<h3>Make PHP File </h3>

* Change the body tag to:
```php
<?php
 
//IP Grabber
 
//Variables
 
$protocol = $_SERVER['SERVER_PROTOCOL'];
$ip = $_SERVER['REMOTE_ADDR'];
$port = $_SERVER['REMOTE_PORT'];
$agent = $_SERVER['HTTP_USER_AGENT'];
$ref = $_SERVER['HTTP_REFERER'];
$hostname = gethostbyaddr($_SERVER['REMOTE_ADDR']);
 
//Print IP, Hostname, Port Number, User Agent and Referer To Log.TXT
 
$fh = fopen('log.txt', 'a');
fwrite($fh, 'IP Address: '."".$ip ."\n");
fwrite($fh, 'Hostname: '."".$hostname ."\n");
fwrite($fh, 'Port Number: '."".$port ."\n");
fwrite($fh, 'User Agent: '."".$agent ."\n");
fwrite($fh, 'HTTP Referer: '."".$ref ."\n\n");
fclose($fh);
?>
```

<h3>Last but not least...</h3>
<p> Before you come and say crap saying i don't know were the ip is go look in the web hosting directory 
or whatever your using and a file called <b>logs.txt</b> will contain all the IPs 

<h1>Go trash talk me on Twitter @thepcmrtim if you have any questions bye.</h1>


