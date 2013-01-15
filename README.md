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

$url    = 'http://www.testurl.de/some/kind/of/path/?and=some&kind=of&query';

$parser = new parseURL($url);
print_r($parser);
echo 'Protocol: '.$parser->get('protocol').'<br />';
echo 'Host: '.$parser->get('host').'<br />';
echo 'Path: '.print_r($parser->get('path'),true).'<br />';
echo 'Query: '.print_r($parser->get('query'),true).'<br />';

?>
```

This would ouput:
```text
Protocol: http
Host: www.testurl.de
Path: Array ( [0] => some [1] => kind [2] => of [3] => path ) 
Query: Array ( [and] => some [kind] => of [query] => 1 ) 
```
