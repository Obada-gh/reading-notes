# Code 301 Reading Notes
hallo there i will sumorize for you some concepts that i learned from html-css book and JS book and How to Write a Git Commit Message from additional resources.
>in the end there is a quiz for you and a map for our info. &#128175;



## How the Web Works (visualization):
When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server.

![visualization](https://www5.0zz0.com/2021/02/27/19/968715239.png)



## Structure : its the page how its looks these are main pionts you need to understand :

* There are three types of HTML lists: ordered,
unordered, and definition.
* Ordered lists use numbers.
* Unordered lists use bullets.
* Definition lists are used to define terminology.
* Lists can be nested inside one another.



## JavaScript and jQuery book by Jon Duckett pages 293-301, 306-331 and 354-357:
jQuery offers a simple way to achieve a variety of common
JavaScript tasks quickly and consistently, across all major
browsers and without any fallback code needed.
When a page loads jQuery from
a CDN, you will often see a
syntax like the one shown below.
It starts with a `<script>` tag that
tries to load the jQuery file from
the CDN. But note that the URL
for the script starts with two
forward slashes (not http:).
liillfill
LOADING JQUERY
FROM A CDN
This is known as a protocol
relative URL. If the user is
looking at the current page
through https, then they will not
see an error that tells them there
are unsecure items on the page.
Note: This does not work locally
with the f i l e:// protocol.
This is often followed by a
second `<script> `tag that
contains a logical operator,
which checks to see if jQuery
has loaded. If it has not loaded,
the browser tries to load the
jQuery script from the same
server as the rest of the website.
```
<script src=" //ajax .googl eapi s . com/ ajax/l i bs/ jquery / 1.10 . 2/ jquery .min. js ">
</ script>
<script>
window .jQuery 11 document. write (' <script src=" j s/j query- 1.10. 2 . j s 11><\jscri pt> ' )
</script>
```
The logical operator looks for
the jQuery object that the
jQuery script makes available.
If it exists, then a truthy value is
returned and the logical operator
short circuits (see p157).
If jQuery has not loaded, then
the document .write () method
is used to add a new `<script>`
tag into the page. This will load a
version of jQuery from the same
server as the rest of the website.
The fallback option is important
because the CDN may be
unavailable, the file may have
moved, and some countries ban
some domain names (such as
Google).
#### example:
![1](https://www4.0zz0.com/2021/04/18/23/535592415.png)

## 6 Reasons for Pair Programming:
1. Greater efficiency
It is a common misconception that pair programming takes a lot longer and is less efficient. In reality, when two people focus on the same code base, it is easier to catch mistakes in the making. Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging (let alone exposing users to a broken product). So, in the long-run, it’s often actually more efficient than two people working on separate features. When coming up with ideas and discussing solutions out loud, two programmers may come to a solution faster than one programmer on their own. Also, when the pair is stuck, both programmers can research the problem and reach a solution faster. Researches also identified pairing enhances technical skills, team communication, and even enjoyability of coding in the workplace.

2. Engaged collaboration
When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. It is harder to procrastinate or get off track when someone else is relying on you to complete the work. Popping open your Facebook timeline is just that less enticing when someone else is looking at your screen.

Another important aspect of learning to program is knowing when to ask for help. We advise our students to spend no more than fifteen minutes stuck on a problem before asking a teaching assistant or instructor for help. When developers pair program, they rely more on each other and can often find a solution together without needing to ask for additional help. Ultimately, this boosts overall confidence.

3. Learning from fellow students
Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would not have thought of. If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution.

Often times, the developers in a pairing have different skill sets. If one programmer is more experienced in a certain skill, they can teach a student who is less familiar with that area. The less experienced developer benefits from the experienced developer’s knowledge and guidance, and the latter benefits from explaining the topic in their own words, further solidifying their own understanding.

4. Social skills
Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities. Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills. When just grabbing the keyboard and taking over isn’t an option, getting good at finding the right words is a skill unto itself.

This has long-term career impacts. As much as employers want strong programmers, they know it’s essential to hire people who can work well with others.

5. Job interview readiness
A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen. They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing code base. By doing so, companies can get a better feel for how an applicant will fit into the team and their collaboration style.

For most roles, the ability to work with and learn from others and stellar communication skills are as (or more!) important to a company than specific technical skills. Pair programming strengthens all of those skills.

6. Work environment readiness
Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.





## JavaScript and jQuery book by Jon Duckett pages 332-335:
Here you can see some of the
jQuery effects that show or hide
elements and their content. You
can animate them fading in and
out, or slide them up and down.
![2](https://www13.0zz0.com/2021/04/18/23/925119654.png)



## JavaScript and jQuery book by Jon Duckett pages 302-305:
jQuery's motto is "Write less, do more," because it allows you to achieve
the same goals but in fewer lines of code than you would need to write
with plain JavaScript.
![3](https://www5.0zz0.com/2021/04/19/00/913465771.png)



## Cheats sheet :

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


## The seven rules of a great Git commit message:
* Keep in mind: This has all been said before.
* Separate subject from body with a blank line.
* Limit the subject line to 50 characters.
* Capitalize the subject line.
* Do not end the subject line with a period.
* Use the imperative mood in the subject line.
* Wrap the body at 72 characters.
* Use the body to explain what and why vs. how.

![4](https://www4.0zz0.com/2021/02/28/22/513821309.png)


## this map for our info :


![map](https://www11.0zz0.com/2021/02/28/00/374479467.png)

## this a quiz for you :
use the images in your page.



>Remember : 
 * FOUCS
 * no pain no gain
 * work hard

### find more :

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
