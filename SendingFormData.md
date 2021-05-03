# Code 301 Reading Notes

hallo there i will sumorize for you some concepts that i learned from html-css book and JS book and How to Write a Git Commit Message from additional resources.
>in the end there is a quiz for you and a map for our info. &#128175;

## How the Web Works (visualization)

When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server.

![visualization](https://www5.0zz0.com/2021/02/27/19/968715239.png)

## Structure : its the page how its looks these are main pionts you need to understand

* There are three types of HTML lists: ordered,
unordered, and definition.
* Ordered lists use numbers.
* Unordered lists use bullets.
* Definition lists are used to define terminology.
* Lists can be nested inside one another.

## Sending form data :
```
<form action="/action_page.php" method="get">
  <label for="fname">First name:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Last name:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <input type="submit" value="Submit">
</form>
```
Definition and Usage
The method attribute specifies how to send form-data (the form-data is sent to the page specified in the action attribute).

The form-data can be sent as URL variables (with method="get") or as HTTP post transaction (with method="post").

Notes on GET:

Appends form-data into the URL in name/value pairs
The length of a URL is limited (about 3000 characters)
Never use GET to send sensitive data! (will be visible in the URL)
Useful for form submissions where a user wants to bookmark the result
GET is better for non-secure data, like query strings in Google
Notes on POST:

Appends form-data inside the body of the HTTP request (data is not shown in URL)
Has no size limitations
Form submissions with POST cannot be bookmarked

### Client/server architecture:
At it's most basic, the web uses a client/server architecture that can be summarized as follows. a client (usually a web browser) sends a request to a server (most of the time a web server like Apache, Nginx, IIS, Tomcat, etc.), using the HTTP protocol. The server answers the request using the same protocol.



![ex](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/client-server.png);



## Cheats sheet

Markdown is a way to style text on the web. You control the display of the document; formaing words as bold or italic, adding images, and creating lists are just a few of the things we can do with Markdown. Mostly, Markdown is just regular text with a few non-alphabetic characters thrown in, like # or *.you just need to make a file with .md extension on Vs code and good to go with this cheats sheet:

 HEADERS :

```

    # This is an <h1> tag
    ## This is an <h2> tag
    ##### This is an <h6> tag

```

list :

```
     orderd:
         1. Item 1
         2. Item 2
         3. Item 3
     unorder:    

         * Item 3a
         * Item 3b

 ```  

EMPHASIS :

```
*This text will be italic*
_This will also be italic_
**This text will be bold**
__This will also be bold__
*You **can** combine them*
```

BLOCKQUOTES :

```
> I’ve always been more interested
> in the future than in the past.
```

> I’ve always been more interested
> in the future than in the past.

LINKS:

```
http://github.com - automatic!
[GitHub](http://github.com)
```

IMAGES :

```
![GitHub Logo](/images/logo.png)
Format: ![Alt Text](url)
```

table :

```
First Header | Second Header
----------- | -------------
Content cell 1 | Content cell 2
Content column 1 | Content column
```

emoji! :

```
:+1: :sparkles: :camel: :tada:
:rocket: :metal: :octocat:
```

for more info : [markdown cheats](https://www.markdownguide.org/cheat-sheet/)

## The seven rules of a great Git commit message

* Keep in mind: This has all been said before.
* Separate subject from body with a blank line.
* Limit the subject line to 50 characters.
* Capitalize the subject line.
* Do not end the subject line with a period.
* Use the imperative mood in the subject line.
* Wrap the body at 72 characters.
* Use the body to explain what and why vs. how.

![4](https://www4.0zz0.com/2021/02/28/22/513821309.png)

## this map for our info

![map](https://www11.0zz0.com/2021/02/28/00/374479467.png)

## this a quiz for you

use the images in your page.

>Remember :

* FOUCS
* no pain no gain
* work hard

### find more

concepts | link
------------ | -------------
 HTML Chapter 1: “Structure” | [Structure](https://obada-gh.github.io/reading-notes-201/Structure)
 HTML Chapter 8: “Extra Markup”| [ExtraMarkup](https://obada-gh.github.io/reading-notes-201/ExtraMarkup)
HTML Chapter 17: “HTML5 Layout” | [Layout](https://obada-gh.github.io/reading-notes-201/Layout)
 HTML Chapter 18: “Process & Design” | [Process & Design](https://obada-gh.github.io/reading-notes-201/Process&Design)
 JS Chapter 1: “The ABC of Programming” | [The ABC of Programming](https://obada-gh.github.io/reading-notes-201/TheABCofProgramming)
 Cheats sheet | [Cheats sheet](https://obada-gh.github.io/reading-notes-201/cheats)

link for the github file : [gitfile](https://github.com/Obada-gh/reading-notes)

##### *writen by OBADA ALHAWJREH.*

My name is obada jaber, I’m 27 years old, I studied Mechanical engineering and i graduated from al balqa applied university, i am now a software student. [OBADA ALHAWJREH](https://github.com/Obada-gh).

##### *Support or Contact:*

Having trouble with Pages? Check out our : [email](obada7jaber7@gmail.com) or phone number : 0781912474 or [contact support for gethub](https://support.github.com/contact) and we’ll help you sort it out. &#x1F691; &#x1F691; &#x1F691;
