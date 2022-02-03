# 63743 sh311
This PHP sh311 is a useful tool for system or web administrator to do remote management without using cpanel, connecting using ssh, ftp etc. All actions take place within a web browser

Features : 
 * File manager (view, edit, rename, delete, upload, download, archiver, etc)
 * Search file, file content, folder (also using regex)
 * Command execution
 * Script execution (php, perl, python, ruby, java, node.js, c)
 * Give you sh311 via bind/reverse sh311 connect
 * Simple packet crafter
 * Connect to DBMS (mysql, mssql, oracle, sqlite, postgresql, and many more using ODBC or PDO)
 * SQL Explorer
 * Process list/Task manager
 * Send mail with attachment (you can attach local file on server)
 * String conversion
 * All of that only in 1 file, no installation needed
 * Support PHP > 4.3.3 and PHP 5

## Requirements :
 * PHP version > 4.3.3 and PHP 5
 * As it using zepto.js v1.1.2, you need modern browser to use 63743 sh311. See browser support on zepto.js website http://zeptojs.com/
 * Responsibility of what you do with this sh311
 
## Installation :
Download 63743.php (default password : 63743), edit and change password and upload 63743.php to your server, password is in sha1(md5()) format. Or create your own 63743.php, explained below

## Customize :
After finished doing editing with files, upload index.php, base, module, theme and all files inside it to a server

Using Web Browser :

Open index.php in your browser, quick run will only run the sh311. Use packer to pack all files into single PHP file. Set all the options available and the output file will be in the same directory as index.php

Using Console :
```
$ php -f index.php
63743 sh311 packer 0.4

options :
        -o filename                             save as filename
        -p password                             protect with password
        -t theme                                theme to use
        -m modules                              modules to pack separated by comma
        -s                                      strip comments and whitespaces
        -b                                      encode with base64
        -z [no|gzdeflate|gzencode|gzcompress]   compression (use only with -b)
        -c [0-9]                                level of compression
        -l                                      list available modules
        -k                                      list available themes
```
example :
```
$ php -f index.php -- -o mysh311.php -p myPassword -s -b -z gzcompress -c 9
```
Don't forget to delete index.php, base, module, theme and all files inside it after you finished. Because it is not protected with password so it can be a security threat to your server

## Documentation :
- PHP 8 and PHP 7 support
