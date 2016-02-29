#API GET Request PHP

This is a simple REST API for translate 'Hello World' in more random language with token security.

#The URL request example:

<a href=''>http://localhost/Hello-World-PHP/HelloWorldPHP.php?token={TOKEN_INPUT}</a>

In the source code, TOKEN_INPUT is md5("Netex"), if you want create private token, you need changed const TOKEN_INPUT = '{YOUR_TOKEN}';
<pre>
<code class="language-php">
  const TOKEN_INPUT = 'YOUR_TOKEN';
</code></pre>

Check request token:

<pre>
<code class="language-php">
  $_GET['token'] == md5(self::TOKEN_INPUT)
</code></pre>


