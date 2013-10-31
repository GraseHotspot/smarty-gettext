## 1.0.1 (unreleased)

IMPROVEMENTS:

  - added manual page for `tsmarty2c.php` (748dbdc from Debian)
  - `tsmarty2c.php` outputs now valid `.po` format (can be used to merge with `.pot`
  - added composer repository. add to your `composer.json`: `"glen/smarty-gettext"`
  - unit tests!

BUG FIXES:

  - Do not show .po file headers on translated pages. (ff6edc6483cc7ebe036b7001d064294545165967, Debian bug: [#680754][1])
  - [PATCH] parse tags properly using {} in parameters (1f044a76, [Kalle Volkov][2])

## 1.0b1 (2005-07-27 Sagi Bashari)

* README:
	- Redone

* smarty-gettext.php:
	- Renamed file to block.t.php

* block.t.php:
	- Rename smarty_translate() to smarty_block_t()
	- Rename strarg() to smarty_gettext_strarg
	- Better comments, new installation method
	- url escaping method

* tsmarty2c.php:
	- Use 'env php' as php bin path
	- Output file name along with ripped strings
	- Comments, wrapping

## 0.9.1 (2004-04-30 Sagi Bashari)

* README: 
	- replace smarty_gettext with smarty-gettext
	- correct package name, project urls, add vrsion

* tsmarty2.c:
	- check if file extension exists before checking if is in array ([Florian Lanthaler][3])
	- correct package name, project urls, add version
	
* smarty_gettext:
	- rename to smarty-gettext
	- correct package name, project urls, add version

## 0.9 (2004-03-01 Sagi Bashari)

* tsmarty2c.php:
	- added support for directories (originally by [Uros Gruber][4])
	- fixed bug that prevented more than 1 block per line (reported by [Eneko Lacunza][5])
	- convert new line to \n in output string

* smarty_gettext.php:
	- run nl2br() when escaping html


  [1]: http://bugs.debian.org/680754
  [2]: mailto:kalle.volkov@hiirepadi.ee
  [3]: mailto:florian@phpbitch.net
  [4]: mailto:uros.gruber@vizija.si
  [5]: mailto:enlar@euskal.org
