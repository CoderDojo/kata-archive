## Summary

 [Ninjas](Ninjas.md) learn to build their first
text-based game using HTML. 

## Tips for use

You will need to either install Scratch on the
[Ninja](Ninja.md)'s machine or use the [web-based
editor](https://scratch.mit.edu/) in advance of using these cards.

## Content

So it's several months later, you've built 10-20 pages and you've got
divs and css and bits of javascript here and there. But it's starting to
get complicated, the pages are difficult to maintain, there is no memory
between pages and it's starting to become boring.

This is where php steps in.

Instead of a room.html for every room we are now going to go back over
all our html files and copy the contents into one file called
message.php.

The contents of each file will go into one position in an array like so

$room\[0\] = "\<div id ='container'\>You are standing outside a castle.
There is a moat.......\</div\>";

$room\[1\] = "\<div id ='container'\>You are inside the
castle.\</div\>";

$room\[2\] ="\<div id ='container'\>You are dead.\</div\>";

How you move from one room to another (from array \[index\] to array
\[index\]) is entirely down to the individual chapters and coder style.
I use an index.php file to jump through case/switch staements and if
statements.

index.php

`  `  
` <?php`  
`    <a href = index2.php?task=”begin”?>Begin the adventure</a>`

index2.php

`  `  
`    <?php`  
`    $response = $_REQUEST; // $_REQUEST takes in the url params and turns them into an array.`  
`    $job = $response[‘task’];`  
`    if ($job ==”begin”){`  
`        echo “You are standing in your room”;`  
`        echo “<a href = index2.php?task=”computer”?>Turn on Your computer</a>”;`  
`        echo “or <br/>”;`  
`        echo “<a href = index2.php?task=”Leave_Room”?>Leave</a>”;`  
`    }`  
`    if ($job ==”computer”)`  
`    {`  
`        //do stuff`  
`    }`  
`    if ($job ==”Leave_Room”)`  
`    {`  
`        //do stuff`  
`    }`  
`    ?>`  
` `

I save the room index locations to each individuals players mysql table,
so they can continue where they left off.

[`How``   ``to``   ``build``   ``a``   ``HTML``   ``game``   ``in`` 
 ``5`` 
 ``lines`](How_to_build_a_HTML_game_in_5_lines.md)`- From Galway Dojo #1,1. Credit: Techbot`  
[`How``   ``to``   ``build``   ``a``   ``HTML``   ``game``   ``in`` 
 ``5``   ``lines``   ``Part``   ``II`` 
 `](How_to_build_a_HTML_game_in_5_lines_Part_II.md)`- From Galway Dojo #1,2. Credit: Techbot`  
[`How``   ``to``   ``build``   ``a``   ``HTML``   ``game``   ``in`` 
 ``5``   ``lines``   ``Part``   ``III`` 
 `](How_to_build_a_HTML_game_in_5_lines_Part_III.md)`- From Galway Dojo #1,3. Credit: Techbot`
