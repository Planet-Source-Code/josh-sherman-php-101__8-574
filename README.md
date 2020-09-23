<div align="center">

## PHP 101


</div>

### Description

Get your feet wet with one of the hottest web languages around, PHP!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Josh Sherman](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/josh-sherman.md)
**Level**          |Beginner
**User Rating**    |4.5 (68 globes from 15 users)
**Compatibility**  |PHP 3\.0, PHP 4\.0
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__8-1.md)
**World**          |[PHP](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/php.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/josh-sherman-php-101__8-574/archive/master.zip)





### Source Code

```
<P align="justify">
So you want to be cool like me and utilize the power of PHP when developing web sites? Then you've come to the right place. This tutorial will give you a basic introduction to PHP, as well as enlighten you to some of the commands that you can use.
</p>
<P align="justify">
If you're curious to what PHP stands for, you're going to be a bit disappointed with my answer. PHP stands for PHP: Hypertext Preprocessor. Now that you're confused, let me explain what PHP is. PHP is a server-side, cross-platform, HTML embedded scripting language. What's that mean to you? It means you can create dynamic web pages!
</p>
<P align="justify">
Before you can start using PHP, you need to find a host that supports PHP, or set it up yourself. PHP is free, and available from <A href="http://www.php.net" target="_blank" class="NAVITEM">http://www.php.net/</a>, along with documentation, functions lists, bugs, et cetera.
</p>
<P align="justify">
Once you have a server at your disposal, you will need a really expensive development environment to code in. Oh wait, we're not talking about a Microsoft product here. All you will need for PHP is a basic text editor. Notepad or vi will be sufficient. As a matter of fact, those are the only tools I use for coding PHP.
</p>
<P align="justify">
Now on to the fun part, hope you're ready to build your first PHP-enabled page.
</p>
<P align="justify">
First, create a new file, and name is "helloworld.php". Note the .php extension. PHP requires files to have a .php, .php3, or .php4 extension. Usually .php will due just fine.
</p>
<P align="justify">
Now I hope you didn't think I was going to skip the infamous "Hello World!" example. Now that you have your file, open it up in your editor, and type in the following code:
</p>
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
<HTML><BR>
   <HEAD><BR>
     <TITLE>Hello World!</TITLE><BR>
   </HEAD><BR>
   <BODY><BR>
     <? echo "Hello World!"; ?><BR>
   </BODY><BR>
</HTML>
</i></b></font></td></tr></table>
<P align="justify">
As you can see, I'm a stickler for indenting, but this is not necessary for PHP.
</p>
<P align="justify">
Once you have the code typed up, go ahead and save the file, upload it to your host, and place it in the appropriate directory on your system, and pull it up in your web browser.
</p>
<P align="justify">
The output should be:
</p>
<P align="center">
<B><I>Hello World!</i></b>
</p>
<P align="justify">
Congratulations you've successfully built your first PHP page. Simple enough, huh? Well that's just a small taste of what PHP can do, and is far from utilizing PHP’s full potential.
</p>
<P align="justify">
Okay, so you've made your first page, big whoop, now it's time to learn what the hell we did. I'm going to go line by line and explain what each bit of code means and does.
</p>
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
<HTML><BR>
   <HEAD><BR>
     <TITLE>Hello World!</TITLE><BR>
   </HEAD><BR>
   <BODY>
</i></b></font></td></tr></table>
<P align="justify">
The first part of the page is simply HTML tags. If you don't know what that does, then I'm sorry for you, and I advise you stop reading this tutorial now and learn some basic HTML.
</p>
<P align="center">
<B><I><? echo "Hello World!"; ?></i></b>
</p>
<P align="justify">
This little bit of code is out only PHP in the entire document. The nice part of PHP is that it gives you the ability to mix and match HTML and PHP to produce a web page.
</p>
<P align="justify">
The <B><?</b>, indicates the start of a PHP tag. Depending on how PHP is set up on your server, you may or may not need to use <B><?php</b> instead of <B><?</b>. To close your PHP tag we use <B>?></b>. PHP tags don't have to be a single line like our page, you can span it over multiple lines, to include more complex code such as if statements and loops.
</p>
<P align="justify">
We've now covered the beginning and ending PHP tags, now we're going to analyze what we have in between them. <B>echo</b> is the command used to print information on the display. Depending on how much you need to display, <B>echo</b> might not be the best choice. For single lines, <B>echo</b> is wonderful, but if you have 2 paragraphs, it may just be better to close the PHP tag and simply have the paragraphs in the HTML portion of the site. <B>echo</b> allows up to display not only plain text that is enclosed in quotes, but variables as well.
</p>
<P align="center">
<B><I>echo $blah;</i></b>
</p>
<P align="justify">
That would output the contents of the <B>$blah</b> variable.
</p>
<P align="justify">
The last portion of the expression is the <B>;</b>. All lines in with <B>;</b> unless they are a part of a conditional expression like an <B>if</b> structure. The rest of the code is just basic HTML to close the BODY and HTML tags, nothing of real importance.
</p>
<P align="justify">
So, you've gotten one page under your belt, and have a basic understanding of how PHP works, and how to use the echo statement. Next, we're going to go over the if statement, and how to create something a bit more dynamic.
</p>
<P align="justify">
Like before, I want you to create a new file, but this time name is "greeting.php". This time, I'm going to walk through the code with you step by step and explain it as we go along.
</p>
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
<HTML><BR>
   <HEAD><BR>
     <TITLE>Greeting!</TITLE><BR>
   </HEAD><BR>
   <BODY>
</i></b></font></td></tr></table>
<P align="justify">
Just like before, we're going to start our page with the basic HTML code, including a title for our site.
</p>
<P align="justify">
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
<? <BR>
   $current_hour = date ("H");
</i></b></font></td></tr></table>
<P align="justify">
Here we opened up our PHP tag, on the next line, we are assigning a variable. The variable is named <B>$current_hour</b>. Variables in PHP start with <B>$</b>, and are case sensitive. The value we are assigning to the variable is <B>date ("H")</b>.
</p>
<P align="justify">
Welcome to the world of functions! <B>date()</b> is a predefined function in PHP that is used to provide with the time and/or date. In this instance, we're pulling the hour of the day, in the 24-hour clock format. The value it assigns to our variable will be 0-23. At the end of our line, we have our semi-colon as usual.
</p>
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
if($current_hour<"12") {<BR>
   echo "Good Morning!";<BR>
}
</i></b></font></td></tr></table>
<P align="justify">
<B>if</b> structures are one of the most useful pieces of code in which you can utilize. In this instance, we are determining if the <B>$current_hour</b> variable is less than 12. If it is less than 12, then we are displaying the words "Good Morning!" and then the structure is complete and it moves on.
</p>
<P align="justify">
<B>if</b> structures are fairly simple, they start with <B>if</b> and within the parentheses, you put in your condition. Your condition can be one of six different operators, <B>==</b> (is equal to), <B>!=</b> (is not equal to), <B>></b> (is greater than), <B><</b> (is less than), <B>>=</b> (is greater than or equal to), <B><=</b> (is less than or equal to).
</p>
<P align="justify">
After we have the <B>if</b> structure put together, we end the line with a fancy bracket, <B>{</b>. The <B>{</b> tells us where to put action code. After we put in the code that will be executed when the condition is met, we end it with the other bracket, <B>}</b>.
</p>
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
if($current_hour<"20" and $current_hour>="12") {<BR>
   echo "Good Afternoon!";<BR>
}
</i></b></font></td></tr></table>
<P align="justify">
This is out second <B>if</b> structure, and incidentally, a little more complex. It contains 2 conditions that have to be met before the result is executed. We separate the conditions with <B>and</b> (you can also use <B>or</b> depending on the situation). If <B>$current_hour</b> is less than 20, and is greater than or equal to 12, then it will display "Good Afternoon!".
</p>
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
if($current_hour>="20") {<BR>
   echo "Good Evening!";<BR>
}
</i></b></font></td></tr></table>
<P align="justify">
The last of our <B>if</b> structures in this page. This one is very similar to our first as it determines if <B>$current_hour</b> is greater than or equal to 20, and displays "Good Evening!" before stopping the PHP tag.
</p>
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
     ?><BR>
   </BODY><BR>
</HTML>
</i></b></font></td></tr></table>
<P align="justify">
Just closing tags. It ends out PHP tag, and the BODY and HTML tags.
</p>
<P align="justify">
All finished, all we need to do is launch the web site and check out the result. Depending on the time of day, you will get a different response, either Good Morning!, Afternoon! or Evening!.
</p>
<P align="justify">
If you've done any kind of programming in other languages, you know that my use of 3 <B>if</b> structures could be refined. That leads me into my next example. No need for a new file this time, we are going to modify "greeting.php" that we just finished up.
</p>
<P align="justify">
Find the following snippet of code, highlight it, and delete it.
</p>
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
if($current_hour<"12") {<BR>
   echo "Good Morning!";<BR>
}<BR>
<BR>
if($current_hour<"20" and $current_hour>="12") {<BR>
   echo "Good Afternoon!";<BR>
}<BR>
<BR>
if($current_hour>="20") {<BR>
   echo "Good Evening!";<BR>
}
</i></b></font></td></tr></table>
<P align="justify">
We are going to rewrite that section of code, and utilize nested if structures.
</p>
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
if($current_hour>="20") {<BR>
   echo "Good Evening!";<BR>
} else {<BR>
   if($current_hour<"12") {<BR>
     echo "Good Morning!";<BR>
   } else {<BR>
     echo "Good Afternoon!";<BR>
   }<BR>
}
</i></b></font></td></tr></table>
<P align="justify">
That will do the same thing as our previous code, but instead of 3 separate <B>if</b> structures, we use 2, and make use of <B>else</b>. <B>else</b> is part of an <B>if</b> structure, which executes a different set of code if the condition is false.
</p>
<P align="justify">
the first <B>if</b> structure checks to see if <B>$current_hour</b> is greater than or equal to 20. If it is, then it displays "Good Evening!". If it isn't then it executes another <B>if</b> structure (our first nested <B>if</b>). That next <B>if</b> structure checks to see if <B>$current_hour</b> is less than 12, and if that is true, then it displays "Good Morning!". If the nested <B>if</b> structure is false, then it displays "Good Afternoon!".
</p>
<P align="justify">
Within the <B>{</b> and <B>}</b> of an <B>if</b> statement, you can put virtually any code you want in there, and it will execute it.
</p>
<P align="justify">
That should do it for using the <B>if</b> structures to create dynamic content. Next on the agenda is to teach you about cases, and query strings, so that you can produce truly dynamic content, instead of just displaying greetings to your visitors.
</p>
<P align="justify">
This next page is going to be called "dynamic.php". Like the first example, I'm going to give you all of the code at once, and then explain it step by step.
</p>
<TABLE align="center"><TR><TD><FONT size="2"><B><I>
<HTML><BR>
   <BODY><BR>
     <?<BR>
        switch ($pageid) {<BR>
          case "1":<BR>
             echo "<TITLE>Page 1</TITLE>";<BR>
             echo "Page 1 content goes here.";<BR>
             break;<BR>
          case "2":<BR>
             echo "<TITLE>Page 2</TITLE>";<BR>
             echo "Page 2 content goes here.";<BR>
             break;<BR>
          case "3":<BR>
             echo "<TITLE>Page 3</TITLE>";<BR>
             echo "Page 3 content goes here.";<BR>
             break;<BR>
          default:<BR>
             echo "Page $pageid doesn't exist.";<BR>
             break;<BR>
        }<BR>
     ?><BR>
   </BODY><BR>
</HTML>
</i></b></font></td></tr></table>
<P align="justify">
Once you have that typed up the code, and put it on your server, bring up the page in your web browser. It should display "Page doesn't exist." What the case statement does, is it allows you to do a large if statement, but not as complicated. The cases are started off by <B>switch ([variable]) {</b>. This determines what variable to check for the cases. In this instance, we are using the variable <B>$pageid</b>. Now each case is defined as <B>case "1":</b> - <B>case "3":</b> and then <B>default:</b>, to represent all over instances.
</p>
<P align="justify">
So we ran it, and it told us the page didn't exist. Why? Because we didn't tell it what page to display, and because of that, it went with the default. This is where the query sting comes in to play for us. I'm sure you've seen a query string in your life time, and if not, oh well, I'm going to explain it anyway.
</p>
<P align="justify">
Pull up the web browser we displayed the page in previously. After the dynamic.php, we're going to append <B>?pageid=1</b> to the end of it. Go ahead and press enter to display that page. This time, it should display "Page 1 content goes here." Now change the <B>pageid=1</b> to <B>pageid=2</b> and then to <B>pageid=3</b>. It should display the appropriate pages for you.
</p>
<P align="justify">
What's all this mean to us as web developers? It means you can have a single file, and host a million different pages off of that file, and make calls to them by a variable in the query string. You can also have multiple variables in the query string, to make your page even more dynamic. The variables can be named virtually anything you want, and are formatted together like this:
</p>
<P align="center">
<B><I>index.php?section=essay&page=2</i></b>
</p>
<P align="justify">
We use the ampersand to separate the variables in the query string. As you can see from the example, you can call the section that you want, and then the page number of that section all from the query string. Once you start to utilize such tricks as this, you will never goes back to coding flat HTML pages.
</p>
<P align="justify">
The other new command is <B>break</b>. <B>break</b> simply stops the execution of a structure, such as our <B>switch</b>, and continues on. We use <B>break</b> at the end of each <B>case</b> so that it doesn't execute all the <B>case</b>s. If we didn't include the <B>break</b>'s, and we ran the page with the query string <B>?pageid=1</b>, then our output would be: "Add content for page 1Add content for page 2Add content for page 3Page 1 doesn't exist. " Not really what we wanted, so we'll stick with the breaks. If you have nested structures, and need to break out of say, 3 of them, you could use <B>break 3;</b> and it will break all 3.
</p>
<P align="justify">
It's almost time to wrap up this tutorial, but I would like to go over a few other simple commands that will help you on your way. First, we have <B>require()</b> which allows you to add text from another file, kind of like server side includes. Unlike <B>date()</b>, <B>require()</b> is not a function in PHP, but a language construct, and doesn't return any value. One great use for <B>require()</b> would be in your cases from the previous code. Instead of adding <B>echo</b> this and <B>echo</b> that, you can have a separate file with all of the code, and then simply have <B>require ("page1.php");</b> which will pull that data into your page.
</p>
<P align="justify">
The last command is <B>exit()</b> which again, is a language construct. <B>exit()</b> will terminate the script and output a message if you want it to. This command is good for detecting an error and halting the script. You can either use <B>exit;</b> to halt it, or something along the lines of <B>exit("Halting Script");</b> to halt it and display "Halting Script" to let the user know what's going on. The nifty part about <B>exit()</b> is that it has an alias. That means there is another command that will do the same exact thing, which is <B>die()</b>. You can use the two interchangeably.
</p>
<P align="justify">
So now you have a basic understanding of how PHP works, and a small knowledge base of commands you can use, along with the basic flow and logic of a page. If you are interested in learning more on your own, check out <A href="http://www.php.net/" target="_blank" class="NAVITEM">http://www.php.net/</a> which has a listing of all the commands, and a full online manual. If that's not enough for you, then search the web, there are quite a few web development sites out there, most of which have information on PHP. If you're too lazy to search on your own, then hold tight, there will be more PHP tutorials in the near future.
</p>
```

