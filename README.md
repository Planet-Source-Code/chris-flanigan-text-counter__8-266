<div align="center">

## Text Counter


</div>

### Description

This code will take a file, who has been initialized by putting 0 in the file and will increment it and display it on a page.
 
### More Info
 
Just do a php include. <?php include "counter.php"; ?>

Make sure your counterfile is read/writeable and that you've initialized it properly.

The if statement in the code is for use with Template Driven Site, another code submission by me. It helps to reduce duplicate hits. You may remove it if you wish.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Chris Flanigan](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/chris-flanigan.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |PHP 3\.0, PHP 4\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__8-1.md)
**World**          |[PHP](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/php.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/chris-flanigan-text-counter__8-266/archive/master.zip)

### API Declarations

Chris Flanigan


### Source Code

```
<?php
if ($do == "") {
	$counterFile="counter.txt";
	$fp= fopen($counterFile,r);
	$num= fgets($fp,5);
	$num +=1;
	$suc=fclose($fp);
	print "<font face=verdana,sans-serif size=1><b>$num</b></font>";
	$fp=fopen($counterFile,w);
	$suc=fputs($fp, $num);
	$suc=fclose ($fp);
} else {
	$counterFile="counter.txt";
	$fp= fopen($counterFile,r);
	$num= fgets($fp,5);
    print "<font face=verdana,sans-serif size=1><b>$num</b></font>";
	$suc=fclose ($fp);
 }
?>
```

