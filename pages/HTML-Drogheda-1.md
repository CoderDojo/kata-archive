## Summary

 A series of five introductory HTML tutorials developed by
CoderDojo Drogheda. Takes you all the way from the basics to the
beginnings of [JavaScript](JavaScript.md). Includes PDF files.


Over the course of the next 3 hours we’ll be running through the basics
of web development\! We’ve broken up the day into different tutorials,
and these will walk you through everything you need to know to get
started making your own websites\! You’ll find each of the tutorials in
the folders on the desktop. Below is a quick rundown of what’s in each
tutorial.

Take your time\! Go at your own pace, if you don’t understand anything,
get stuck or have any questions there’s lots of us on hand to help you
out\! (and if you find the pace a bit too slow we’ll find something for
you to challenge you\!)

## Before you begin

You will need your favourite code editor to create your HTML files. Try
SciTE for Windows or Linux available at
<http://www.scintilla.org/SciTEDownload.html> (download the 'full
download' under 'Windows Excecutable') Or Komodo Edit for
Mac/Windows/Linux available at <http://www.activestate.com/komodo-edit>

## Tutorial 1

Your first web page\! This will take you through what you need to make a
web page, and making your first web page\!

[file:HTML\_Tutorial\_1.pdf](file:HTML_Tutorial_1.pdf.md)

A guy called Tim Berners Lee is the man you can thank for everything on
the World Wide Web. In 1990 he invented this language called HTML which
is still used today\! If ya open up your web browser, right click on the
page and hit View Source you’ll see a whole load of mad things wrapped
in more than and less than signs. This is HTML, or as you’ll see in the
source

<html>

.

Depending on the website you went on, it probably looks like a total
mess that you’d never make sense of\! But don’t worry, it’s really
really simple.

HTML stands for Hyper Text Markup Language. It’s based around the idea,
that your internet browser can read these “markup tags”. In English that
means, if in your web page you have something like <strong>My text is
bold</strong> your browser will show you the text My text is bold (in
bold just like that\!)

Getting Started

Right let’s get to it\!

There are millions of tools you can use to make web sites, but we’re
gona start off with a really simple one. There’s an icon on your desktop
called SciTe. When you open it, it’ll be blank, and

you’ll be able to type into it\!

We call this a Text Editor. Because you can… edit text in it…
Programmers use text editors to write their programs in. They’re really
handy because they’ll highlight your code making it really easy to

read\!

Your first web page

This is really simple\! Go to file, save as, and save your blank file as
“index.html” (without the quotation marks) and save it to the desktop.

Congrats\! Now on your desktop you’ll have a blank webpage\! But how do
we put stuff into it?

If you go back to SciTe, you can just type any text you like save it,
and now your page will have that text in it\! But that makes it really
boring and you can’t do much like that\!

So let’s introduce a few tags. Every web page should start off like
this:

<html>

<head>

<title>

My First Web Page

</title>

</head>

<body>

</body>

</html>

We’ll explain on the next\!

You’ll notice that all of these tag things are placed in order, so the

<html>

tag wraps around everything on the page. This is the way the tags work.
You open a tag with <tag> and end it with

</tag> when you want to close it.

If you type the code into SciTE and open up the page in your browser
you’ll see its still blank\! But in the bar at the very very top of
the browser you’ll see “My Frist Web Page”\! This is whats going on with
the head and title parts\! So

<head>

tells the browser everything between

<head>

and

</head>

is to do with whats going on up there. But what about between

<body>

and

</body>

??

This is where the exiting stuff happens\!

Headings and Paragraphs

If you type text between

<body>

and

</body>

this will tell the browser to show that text\! But it still looks a bit
bunched up and together.

Try adding <hl>My first heading</hl> in between the body tag, save it,
and refresh your page to see what happens\! (It should be big and black
and bold\!)

But what about separating out text after that? Well, try adding in a
paragraph\! Wrap some text in a p tag\! Like this:

your text

after the closing h1 tag\! So you should end up with something that
looks like this:

Images

Go to google and search for an image of something ya like. Save the
image to the deskop, and make sure you take note of its name and file
type\! (So you’re looking for “myimage.jpg” or “myimage.png”) If you
want to put this image onto your web page, you have to do something a
bit more complicated. The image tag is <img> but to add the image, you
have to tell the browser where the image
is.

`To do this, you have to add an attribute to the tag. For an image, you have to tell the browser where the source is. So your image tag is `<img src=”myimage.png”>`, where myimage.png is the name of your image! But what about the closing tag? Well, because you’ve nothing to go inbetween it, you can use the shorthand version, so your tag becomes `<img src=”myimage.jpg” />

That’s it\! Save it and refresh your page, your image should now be
there\!

## Tutorial 2

[file:HTML\_Tutorial\_2.pdf](file:HTML_Tutorial_2.pdf.md)

Tables and Lists\! Ok, so you have your first web page, but what if you
have a table of stuff to make? How about a list of items? A guy called
Tim Berners Lee is the man you can thank for everything on the World
Wide Web. In 1990 he invented this language called HTML which is still
used today\! If ya open up your web browser, right click on the page and
hit View Source you’ll see a whole load of mad things wrapped in more
than and less than signs. This is HTML, or as you’ll see in the source

<html>

.

Depending on the website you went on, it probably looks like a total
mess that you’d never make sense of\! But don’t worry, it’s really
really simple.

H If you type the code into SciTE and open up the page in your browser
you’ll see its still blank\! But in the bar at the very very top of the
browser you’ll see “My Frist Web Page”\! This is whats going on with the
head and title parts\! So

<head>

tells the browser everything between

<head>

and

</head>

is to do with whats going on up there. But what about between

<body>

and

</body>

??

This is where the exiting stuff happens\!

Headings and Paragraphs

If you type text between

<body>

and

</body>

this will tell the browser to show that text\! But it still looks a bit
bunched up and together.

Try adding <hl>My first heading</hl> in between the body tag, save it,
and refresh your page to see what happens\! (It should be big and black
and bold\!)

But what about separating out text after that? Well, try adding in a
paragraph\! Wrap some text in a p tag\! Like this:

your text

after the closing h1 tag\! So you should end up with something that

looks like this:

Images

Go to google and search for an image of something ya like. Save the
image to the deskop, and make sure you take note of its name and file
type\! (So you’re looking for “myimage.jpg” or “myimage.png”)

If you want to put this image onto your web page, you have to do
something a bit more complicated. The image tag is <img> but to add the
image, you have to tell the browser where the image
is.

`To do this, you have to add an attribute to the tag. For an image, you have to tell the browser where the source is. So your image tag is `<img src=”myimage.png”>`, where myimage.png is the name of `

your image\! But what about the closing tag? Well, because you’ve
nothing to go inbetween it, you can use the shorthand version, so your
tag becomes <img src=”myimage.jpg” />

That’s it\! Save it and refresh your page, your image should now be
there\!

## Tutorial 3

[Media:HTML\_Tutorial\_3.pdf](Media:HTML_Tutorial_3.pdf.md)

Not so black and white anymore\! Adding CSS, or styling to your web page
so it has colours and a bit more life\!
[Media:Tutorial\_3.pdf](Media:Tutorial_3.pdf.md)

Time to get a bit artzy\!

So now we have a web page with a heading, a paragraph, an image, a list,
and a table. But it’s all a bit boring looking. Let’s put some life into
it

CSS

Cascading Style Sheets is the second language we’ll introduce. This is
the language we use to add colour, fonts, background images, padding,
margins…..and lots more\! It’s incredibly simple to get

started using it. For this, we first need to add a style tag to the head
with the attribute type=”text/css”\! You can add this to your existing
web page, so you should have something like:

<html>

<head>

<title>

My first web page

</title>

<style type=”text/css”>

</head>

<body>

….

</body>

</html>

Adding colour and fonts\!

The format for adding CSS is different to HTML tags. It revolves around
the idea that you select different tags, or named elements and then
apply styles. We’ll start with a simple example of changing the colour
and font of the heading\! Within the style tag in the head add:

h1 {

`color: #FF0000; `  
`font-family: san-serif; `

}

So the above tells your browser that it should find all the h1 tags in
your page, and change the colour to red, with a san-serif font. A
san-serif font is a font without all the added feet and other trims. So
it looks something like this. You can name a font if you like, just make
sure its installed on your machine otherwise it won’t show up\!

The font colours are done in “hex” format. Hex is a numbering system,
you can find a reference of colours here:
<http://www.december.com/html/spec/colorsafe.html> (and thats not a
typo, you have to use the American spelling of colour\!\!)

You can do the same with all tags. So for the list or the paragraph, add
the same code again, but replace the h1 with “li” or “p”.

Single Element Selection

But what if you want to just select a single element in your list and
apply a certain colour to it, but not apply it to the entire list? Well,
there’s two says to do this depending on if you want to only apply it to
one, or multiple. For this we need to introduce the idea of an id and a
class. An id is a unique identity for the element. So you should only
use it once\! But a class can be used

multiple times for as many elements as you like\! To apply it to your
list items it looks like this:

  - The Black Sheep
  - Sheep 1
  - Sheep 2
  - Sheep 3
  - Just a regular list item

You can name your ids and classes whatever you like\! But they can only
be made up of numbers, letters and dashes “-“. On the CSS side of things
we have to add a bit more though. For an id you need to add the prefix
\# and for a class it’s a dot. So to apply styling to the above, all I
need to do is:

` #uniqueElement { `  
`color: #000000; `  
`font-family: san-serif; `  
`} `

ommonStyle {

`color: #EEEEEE; `  
`font-family: san-serif; `  
`} `

Simple\!

Background Colours

Background colours are just as easy as regular colours, you just use
background-color: \#EEEEEE;

For example, if you want to set the background colour of a list item,
you just need to add something like:

` #uniqueElement { `

` color: #000000; `  
` background-color: #EEEEEE; `  
` font-family: san-serif; `  
` } `

Other style attributes

Have a play around with the different style attributes below, and see
what you can come up with\!

(What’s inside the square brackets are examples of the different vales
you can enter\!)

`.className { `

`color: #ff0000; `  
`font-family: san-serif; `  
`background-color: #eeeeee; `  
`font-size: 12px; `  
`font-weight: [bold, regular]; `  
`text-decoration: [underline, overline, line-through, none]; `  
`padding: 5px; `  
`padding-left: 5px; `  
`padding-right: 5px; `  
`padding-top: 5px; `  
`padding-bottom: 5px; `  
`margin: 5px; `  
`margin-top: 5px; `  
`margin-bottom: 5px; `  
`margin-left: 5px; `  
`margin-right: 5px; `  
`width: 100px; `  
`height: 100px; `  
`border: solid 1px #eeeeee; `  
`border-top: solid 1px #eeeeee; `  
`border-bottom: solid 1px #eeeeee; `  
`border-left: solid 1px #eeeeee; `  
`border-right: solid 1px #eeeeee; `  
`}`

## Tutorial 4

[file:HTML\_Tutorial\_4.pdf](file:HTML_Tutorial_4.pdf.md)

Time to get serious\! (Kinda…)

Believe it or not, if you’ve made it this far, you now only need one
more thing to make an actual website\! At the moment you have a web
page. But to have a website, you need to have more than one\! Just go
file save as, and save page2.html (or somethingmoremeaningful.html).
BHAM\! Two web pages, that’s a website\! But how the heck do you get
from one page to another?

Links

In order to link them together you need to use an “a” tag. Below is the
example code on how to link pages together. You can wrap this around
text or images, and it will become a link to another webpage\!

`  `<a href=”myotherpage.html”>`My Link to my other page`</a>` `

And that’s it\! That’s all the tools you need to make a website\!\!

Challenge time\!

Right\! Now that you’ve got more than one page, you’ve got them linking
together, you know how to make a heading, a paragraph, a list, an image,
and how to style of them together. Delete everything you’ve done\!
Seriously…

Start from scratch. But this time, use everything you’ve learned from
these tutorials to make your own actual website. Pick a topic you’re
interested in, sport, movies, music, and make a website about that, (you
can copy and paste the information from other websites online if you
like\!).

We recommend that you format it like the following:

Heading

`   `<hl>`List with links to your other pages `  
`  `

,

<li>

,<a>

(this will become your menu, we’ll show you how\!\!)

Paragraph of text and images

,<img>.

Footer with your copyright. (the copyright symbol can be typed in by
using ©).

Make your home page first. We’ll show you how to turn the list into a
menu that goes across the page without the bullet points, then plough
ahead with the rest of your site\! Try and get at least 5 pages\! All
mad ideas are welcome, we’ll do our best to show you how to do them\!

## Tutorial 5

[file:HTML\_Tutorial\_5.pdf](file:HTML_Tutorial_5.pdf.md)

So you have a website now\! Let’s make thing complicated and bring in a
third language\!
[Media:Tutorial\_5.pdf](Media:Tutorial_5.pdf.md) This is where
we get really really complicated\! You’re about to get a crash course in
events and

logic while learning another language\! Javascript. But this is also
where things start to get really fun, because theres Javascript is what
enables you to interact with your webpage, so your content can change as
you start to use your website.

### Getting Started

Long ago, way back when Google was just a computer up to your knee
sitting in a garage somewhere, Javascript was complicated, and mean, and
horrible, and took the joy out of all the fun things you could do with
it. But thankfully, we now have these things called Frameworks. These
were invented to make coding easier\! They basically take all the
complicated bits, wrap them in a much nicer to use code, and let you get
all the benefits, without all the headaches\! The framework we’ll be
using today is jQuery.

To get started, first we have to include the jQuery framework. To do
this, you need to introduce a “script” tag to the head of your web page
as below:

`   <script type=”text/javascript”`

`   src=”http:// 'example.com'”>`

</script>

You now have the jQuery framework added\!

### On Load

Events\! On Load is one of the most important events, because without
it, jQuery wouldn’t work properly\! Lets start with a simple example.
Once the page loads, we want an alert box to appear saying “Hello
World\!” (- if you go onto college to do programming, the first program
you’ll ever write should contain the words Hello World, it’s a tradition
we programmers have, when we learn a

new language, we get it today Hello World.)

To do this, its easy. First we open up a new script tag in the head,
just like we did to include the framework. But instead of setting a src
attribute, we’re going to write our javascript code inside the

script tag\! So it will look something like this:

<script type=”text/javascript”>

`   $(document).ready(function() `  
`   { `  
`       alert(“Hello World”); `  
`   }); `  
`  `

</script>

So, what we have here, is a small piece of javascript code which says,
when the document is ready, alert the words Hello World. The crazy
amounts of brackets are very important\! Everything you do

in javascript is wrapped around those brackets, much like how you have
closing tags in HTML.

### On Click

Right, lets try do something a bit more complicated. Lets say you have a
link on a page, and when you click this link, you want the content in
the box below it to change its text, and its colour. So for

this, we’ll need a link, and a box in the body part of our HTML, like
this:

`  `<a href=”javascript:;” id=”mybutton”>`Click me`</a>` `

<div id=”mycontent”>

Click above, to see me change\!

</div>

A div is just a box, with no special properties like a table or
paragraph, just a way of sectioning off, or dividing content, or in our
case, making a box\!

Ok, now we have our button saying Click me, it’s a regular link like you
already know how to do, but the href part, where you normally put
another page address has this javascript:; thing in it.

That’s to make sure that when a person clicks on it, the browser doesn’t
bring the user to another page, we want them to stay on the same page,
while we change whats in the mycontent box. We’ve given the link an id
of mybutton. We’ll need this, much like we need it in CSS to change its
styles, so that we can add the event to it, that once the link is
pressed the box below it changes

colour and its content. So in javascript we have to:

1\. Wait for the page to load

2\. Add an event to \#mybutton when its clicked

a. If the event is called, \#mycontent needs to change its text colour,
and change its

content.

The code for this is: (it again goes in the head)

<script type=”text/javascript”>

`   $(document).ready(function() {`  
`   $(‘#mybutton’).click(function() `  
`   { `  
`     $(‘#mycontent’).text(‘My content has changed now!’); `  
`   }); `  
`   }); `  
`   `

</script>

Have a play around with this and see what you can come up with\! Other
events like .click are .mouseenter .mouseout

Try using the .attr to change the src of an image
$(‘\#myimage’).attr(‘src’, ‘newimage.jpg’);

Call us over if you think you’re ready to try animations\!\!

`   $(‘#mycontent’).css({‘color’:’#FF0000’ });`
