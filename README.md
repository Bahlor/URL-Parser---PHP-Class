URL-Parser---PHP-Class
======================

A php class for parsing urls very simply. Feel free to contribute. :)

Freely distributable under the MIT License.

## Basic example
================

Lets take the following example:

```php
<?php
include('urlparser.class.php');

$url    = 'https://github.com/Bahlor/URL-Parser---PHP-Class/';

$parser = new parseURL($url);

echo 'Protocol: '.$parser->get('protocol').'<br />';
echo 'Host: '.$parser->get('host').'<br />';
echo 'Path: '.print_r($parser->get('path'),true).'<br />';
echo 'Query: '.print_r($parser->get('query'),true).'<br />';

?>
```

This would ouput:
```text
Protocol: https
Host: github.com
Path: Array ( [0] => Bahlor [1] => URL-Parser---PHP-Class )
Query: 
```
