## Summary

 How to build an HTML game in 5 lines.
[Ninjas](Ninjas.md) learn to build their first text-based
adventure game using HTML. The game consists of a series of web pages
where each page is one step/room in the story. 1hr 15mins.


## Content

### Week1

We ignored body tags and such. We can deal with doing things correctly
after learning how to
do.

So.

  - index.html

`   My name is <b>Techbot</b>`

becomes

`   My name is <i>Techbot</i>`

becomes

`   `  
`    You are standing in front of a castle surrounded by a <b>shark filled</b> moat. You can <i>enter</i> the castle or <i>jump</i> in the moat.`  
`  `  
`    <a href ="room1.html">Enter</a> or <a href="room2.html"> Jump </a>`

  - room1.html

`   you are in the castle <br/>`  
`    <img src="castle.jpg">`

  - room2.html

`   You are dead`

This took roughly an hour and fifteen minutes per class, taking into
account:

  - Windows OS not showing extensions by default.

<!-- end list -->

  - Some issues with editing html files on a MacOS with the default
    editor.

<!-- end list -->

  - Standard typos

<!-- end list -->

  - Giving the kids from 10-20 minutes (up to 6 months)to expand on the
    idea.

![escape.png](../files/img/escape.png "escape.png")

### Week2

Embedding inline css to centre both the text and image and create a
border

#### Step 1

we create a "container" to house our elements. At present the container
has no attributes so when you refresh in the browser you see no changes.
Our cotainer is called a division and looks like this

<div>

some
code

</div>

`   `  
` <div> `  
`  `  
` You are standing in front of a castle surrounded by a <b>shark filled</b> moat. You can <i>enter</i> the castle or <i>jump</i> in the moat.`  
`  `  
`    <a href ="room1.html">Enter</a> or <a href="room2.html"> Jump </a>`  
` </div>`

#### Step 2

we give our div a width, and a
border.

`   `  
` <div "style = `  
`width: 500px;`  
`border: 1px red solid;`  
`> `  
`  `  
` You are standing in front of a castle surrounded by a <b>shark filled</b> moat. You can <i>enter</i> the castle or <i>jump</i> in the moat.`  
`  `  
`    <a href ="room1.html">Enter</a> or <a href="room2.html"> Jump </a>`  
` </div>`

#### Step 3

Finally we add a margin , we can use four numbers 1 for top, 1 for
bottom, 1 for left and 1 for right. Or we can use two numbers: 1 for top
and bottom, and 1 for left and right.

We can also replace the number with auto, which has the effect of
centering the
div

`  `  
` <div "style = `  
`width: 500px;`  
`border: 1px red solid;`  
`margin: 0 auto;"`  
`> `  
`  `  
` You are standing in front of a castle surrounded by a <b>shark filled</b> moat. You can <i>enter</i> the castle or <i>jump</i> in the moat.`  
`  `  
`    <a href ="room1.html">Enter</a> or <a href="room2.html"> Jump </a>`  
` </div>`

[`How``   ``to``   ``build``   ``a``   ``HTML``   ``game``   ``in`` 
 ``5`` 
 ``lines`](How_to_build_a_HTML_game_in_5_lines.md)`- From Galway Dojo #1,1. Credit: Techbot`  
[`How``   ``to``   ``build``   ``a``   ``HTML``   ``game``   ``in`` 
 ``5``   ``lines``   ``Part``   ``II`` 
 `](How_to_build_a_HTML_game_in_5_lines_Part_II.md)`- From Galway Dojo #1,2. Credit: Techbot`  
[`How``   ``to``   ``build``   ``a``   ``HTML``   ``game``   ``in`` 
 ``5``   ``lines``   ``Part``   ``III`` 
 `](How_to_build_a_HTML_game_in_5_lines_Part_III.md)`- From Galway Dojo #1,3. Credit: Techbot`
