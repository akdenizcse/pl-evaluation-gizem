# PHP

PHP is an open-source server-side scripting language which is used for implementing dynamic and interactive Web pages.

**What is PHP?**

PHP is an acronym for "PHP: Hypertext Preprocessor" which is embedded with HTML. Its structure was influenced by many languages like C, Perl, Java, C++, and Python.

The mascot of the PHP is a blue elePHPant, designed by Vincent Pontier in 1998.

**History of the PHP**

Rasmus Lerdorf  wrote his personal homepage with C programming language which is  connected with web forms and databases in 1994 and called  "Personal Home Page/Forms Interpreter". Then Lerdorf released of PHP/FI as "Personal Home Page Tools (PHP Tools) version 1.0" in 1995. Today, it is improved by the PHP Group. 

-PHP 2 : It was released in 1997 

-PHP 3 and 4  : Development moves from one person to multiple developers for PHP 3 in 1998. PHP 4 is  powered by the Zend Engine, was released in 2000.

-PHP 5 :It was released in 2004 and it included new features such as improved support for object-oriented programming and the PHP Data Objects (PDO).

-PHP 6 : Not released new version,  it is supported Unicode.

-PHP 7: The version 7 was developed in 2014-2015
 
-Latest versions of PHP are PHP 7.2.29, PHP 7.3.16 and PHP 7.4.4 released in 2020.
 
Note: PHP Development Team created a system for timeline of the releases PHP. Under this system, at least one release should occur every month and once per year, a minor release should occur which may include new features. Every minor release should be supported for two years with security and bug fixes, and at least one year of only security fixes, for a total of a three-year release process for every minor release.
 
**PHP File**

PHP files can contain text, HTML, CSS, JavaScript, and PHP code is executed on the server, and it is returned to the HTML file in the browser. PHP files have extension “.php"

**Why was it invented ?**

It was developed for basic web development but now it is used as a general-puporse languages. For example 

-Generate dynamic page content

-Create, open, read, write, delete, and close files on the server

-Collect form data

-Access cookies variables and set cookies

-Add, delete, modify data in your database

-Used to control user-access

-Encrypt data

Users can output HTML, images, PDF files, and Flash movies with PHP, also the output can be any text, such as XHTML and XML.

**When/why shall we use it ?**

Developers prefer it because
-PHP runs on various platforms (Windows, Linux, Unix, Mac OS X, etc.)
-PHP is can compatible with all servers used today (Apache, IIS, etc.)
-PHP supports databases such as MySQL, PostgreSQL, Oracle, Sybase, Informix, and Microsoft SQL Server.
-PHP is free.
-PHP is easy to learn and runs efficiently on the server side.
-PHP supports some protocols such as POP3, IMAP, and LDAP. 

And also PHP has five important characteristics:
-Simplicity
-Efficiency
-Security
-Flexibility
-Familiarity

**PHP Syntax**

-A PHP script is executed on the server and result is sent back to the browser in HTML format. 

-A PHP script can be placed anywhere in the document.

-A PHP script starts with

 ```
 <?php
 // PHP code goes here
 ?>
 ```

-Filename extensions are ".php, .phtml, .php3, .php4, .php5, .php7, .phps, .php-s, .pht, .phar".

-PHP statements end with a semicolon (;).

**How to setup an environment to use it in different platforms?**

Three  main components need to be installed for develop and run PHP web pages

-Web Server: PHP will work with virtually all Web Server software, Microsoft's Internet Information Server (IIS) but usually used is freely available Apache Server. 

-Database: PHP will work with virtually all database software, including Oracle and Sybase but generally used is freely available MySQL database.

-PHP Parser: A parser must be installed to generate HTML output that can be sent to the Web Browser.

Linux : If the desktop runs on Linux, these are have to be installed 

-Apache or Lighttpd

-PHP

-MySQL or Postgresql

-The PHP integration plugin for the database.

Mac OS X:  It does come with PHP. To install MySQL and run the OS X installer package manager such as Homebrew, Macports or use MAMP, XAMPP. Also users can be use phpbrew, it is a tool for installing and managing multiple PHP versions.

Windows : When users have  a servers( Apache web server or  Internet Information Services (IIS) server from Microsoft) installed, users can download and install the PHP for Windows. 
Databases : On Microsoft Windows users must always install own database. Two popular choices are the open source Postgres, and MySQL. 
Also, a package installer called WAMPserver is available. It simply installs Apache, PHP and MySQL.

**PHP frameworks**

Most developers prefer to use frameworks for the web development. The advantage of using a framework is following the best practices of the language and using MVC pattern.

Examples of popular PHP frameworks

-CodeIgniter

-Laravel

-Symfony

-Zend

-CakePHP

-FuelPHP

-Slim

-Yii 2

**Some PHP Example Codes**

Some basic/specific PHP string functions 

- Users can reverse a string using the strrev() function. 

```
<?php
echo strrev("Programming Languages"); 
?>
```
Output: 
```
segaugnaL gnimmargorP
```

- Users can use str_replace() function for replace text within a string

```
<?php
echo str_replace("Programming", "Languages", "Programming Interpreted"); 
?>
```
Output:
```
Interpreted Languages 
```

-The rsort() functions sort the values of an array in descending alphabetical/numerical order (Ex: Z, Y, X, W, V... 5, 4, 3, 2, 1...)

```
<?php
$languages = array("PHP", "code");
rsort($languages);
print_r($languages);
?>
```

Output:
```
Array
(
   [0] => PHP
   [1] => code
)
```

-The asort() function sorts an associative array, by it's values, in ascending alphabetical/numerical order (Ex: A, B, C, D, E... 5, 4, 3, 2, 1...)

- The ksort() function sorts an associative array, by it's keys, in ascending alphabetical/numerical order (Ex: A, B, C, D, E... 5, 4, 3, 2, 1...)

```
<?php
$languages = array("zero"=>"PHP", "one"=>"code");
ksort($languages);
print_r($languages);
?>
```

Output:

```
Array
(
   [one] => code
   [zero] => PHP
    
)
```
- The arsort() function sorts an associative array, by it's values, in descending alphabetical/numerical order (Example. Z, Y, X, W, V... 5, 4, 3, 2, 1...)

- The krsort() function sorts an associative array, by it's keys in descending alphabetical/numerical order (Example Z, Y, X, W, V... 5, 4, 3, 2, 1...)

```
<?php
$languages = array("zero"=>"PHP", "one"=>"code", "two"=>"call");
krsort($languages);
print_r($languages);
?>
```

Output:

```
Array
(
    [zero] => PHP
    [two] => call
    [one] => code
)
```
**Forms**

Forms are used for users to enter data or select data from the webpage. To create a form with PHP users need some attributes in html. PHP uses 'post' and 'get' global variables to get the data from form.

```
<html>
<body>
  <form method="get" action="target_proccessor.php">
      <input type="search" name="search" /><br />
      <input type="submit" name="submit" value="Search" /><br />
  </form>
<body>
</html>
```

The 'method' attribute here tell the form the way to send the form data. Then the 'action' attribute tell where to send form data to process. The 'name' attribute should be unique because in php the value of the name work as the identity of that input field.

-Checking Required Inputs
PHP has a few functions to check if the required inputs have been met. Those functions are isset, empty, and is_numeric.

-Checking form to make sure its set
The isset checks to see if the field has been set and isn't null. Example:
```
$firstName = $_GET['firstName']

if(isset($firstName)){
  echo "firstName field is set". "<br>";
}
else{
  echo "The field is not set."."<br>";
}
```

-Handling Form Input
Users can get form inputs with global variables $POST and $GET.
`$_POST["firstname"]` or `$_GET['lastname']`

**Security**

-In 2019, 11% of all vulnerabilities listed by the National Vulnerability Database were linked to PHP; historically, about 30% of all vulnerabilities listed since 1996 in this database are linked to PHP. 

-In a 2013 analysis of over 170,000 website defacements, published by Zone-H, the most frequently (53%) used technique was exploitation of file inclusion vulnerability, mostly related to insecure usage of the PHP functions include, require, and allow_url_fopen.

**Things that are specific to this language?**

-Php is a multi-paradigm languages(imperative, object-oriented).

-PHP has several levels of error severity. The three most common types of messages are errors, notices and warnings. These have different levels of severity; E_ERROR, E_NOTICE, and E_WARNING.

-PHP is an “exception-light” programming language.It means, it will try to keep processing regardless even a fatal error occurs.

-As of May 2020, PHP is used by 78.4% of all the websites whose server-side programming language we know.

-The largest Social Networking Platform, Facebook is written using PHP.

 

**References:**

-[W3Techs](https://w3techs.com/technologies/history_overview/programming_language/ms/y)

-[ResearchGate](https://www.researchgate.net/figure/Examples-of-PHP-JSP-and-ASPNET-scripts-with-HTML_tbl2_256404467)

-[WikiBooks](https://en.wikibooks.org/wiki/PHP_Programming)

-[PHP.net](https://www.php.net/docs.php)

-[Wikipedia](https://en.wikipedia.org/wiki/PHP)

-[w3school](https://www.w3schools.com/php/default.asp)

-[TutorialsPoint](https://www.tutorialspoint.com/php/index.htm)

-[FreeCodeCamp](freecodecamp.org/news/the-best-php-examples/)

