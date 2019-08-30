Because of canvas rotation using translate and transform. I am building
three different but similar shoot 'em ups to examine the obstacles etc.
I started off copy and pasting the platform game loop from template003
to four new repos. I want to examine both the similarities and changes
within these four loops and also also for a small bit of repetition
within the code to allow myself and fellow ninjas become more acquainted
with whatever new javascript commands or constructs I come
across.

`  * This is a work in progress,which  means the code will be bloated with stuff that is no longer relevant.`  
`  * A function may be optimised in one game loop, but has not in another (yet). `  
`  * Like the Javascript adventure game there will be branches with `**`expanded`**` code in the future.`  
`  * These main loops are not written in an object oriented fashion but rather as simplistic functions.`  
`  * They are intended to follow on from a very simple text adventure. `  
`  * There may be oop styled code to follow in expanded branches of these games.`  
`  * Most likely the next set of game loops will be written in an oop fashion.`  

After moving the code around to facilitate each of the shooters, one
using rotate canvas , one using \[bounds map image\], a bit of tweaking
and adding loads of global variables. I finally moved half the code out
of the single function - the ubiquitous draw() as powered by Paul Irish
and into a function : update().

I've added a shoot function that only goes 20 units from the spaceship
before disappearing. I used the square root of x squared minus x2
squared plus y minus y2 all to be squared to work out the distance
between the bullet and the shooter. I made this for the simple canvas
game and just added it her for future use. I was the first time I ever
used that equation outside of school.

[file:Multi-dim-battle.png](file:Multi-dim-battle.png.md)

`template013`  
`*multidirection shoot 'em-up`  
`*`<https://github.com/Techbot/template013>  
`* `[`-Demo-`](http://techbot.github.io/template013/)

To rotate a single object(in this case the hero spaceship). We rotate
the whole canvas print the spaceship and then rotate back. This might
seem like a thing to avoid(why can't I just rotate the spaceship?), but
in the end it actually amounts to the same
thing.

` context.drawImage(background_obj, backg_x, backg_y);`  
` context.save(); // prepare for rotation`  
` context.beginPath();// begin`  
` context.translate( 290,210 );Move to the centre of the hero spaceship`  
` context.rotate(degrees*Math.PI/180);// rotate the whole canvas`  
` context.drawImage(imageObj, -37, -50);// draw the hero`  
` context.restore();// rotate back to save`  
` context.drawImage(imageObj2, x2, y2);// continue drawing stuff`  
` context.drawImage(imageObj3, x3, y3);`

[file:Dojo\_racer\_battle.png](file:Dojo_racer_battle.png.md)

`template012`  
`*single direction racer`  
`*`<https://github.com/Techbot/template012>  
`* `[`-Demo-`](http://techbot.github.io/template012/)

Although orinally inspired by the ultrasimple dojoracer scratch game by
coderdojoseatle seen here
<http://kata.coderdojo.com/wiki/ScratchTastic#DojoRacer> . I predicted
(correctly) my first interesting code conundrum. We are all used to

`   x = x + 1 or x= x+ dirX`

(where dirX equals 1 or -1) for incrementing the x axis position

or

`  y = y + 1 or y= y+ dirY `

(where dirY equals 1 or -1) for incrementing the y axis position

But in this case we need to update the x and y axis based on the
direction the car is facing. What do we do? We go to stackoverflow of
course. One of the tricks for speeding up coding is

  - (a)recognising if the code conundrum is one that other coders have
    likely come across and discussed before.
  - (b) phrasing your question so that it will come up i a search engine
    or if really necessary for posting.

So a few minutes later we are here :
<http://stackoverflow.com/questions/19355026/move-an-object-in-the-direction-its-facing-using-2d-html5canvas-and-ctx-rotate-f>

and there's the clue:

`       this.x +=   this.speed * Math.cos(angle * Math.PI / 180);`  
`       this.y -=   this.speed * Math.sin(angle * Math.PI / 180); `

[file:shooter.png](file:shooter.png.md)

`template011`  
`* `<https://github.com/Techbot/template011>  
`* Simple shoot 'em up`  
`* `[`-Demo-`](http://techbot.github.io/template011/)

The first iteration of this game loop proved annoyingly difficult. I'm
using a modified version of the imagebounds png as used in canvas hero
<http://www.html5canvastutorials.com/cookbook>

But by the time a non-boundary ie black pixel was thrown up, it was too
late.a nd hus the spaceship would get stuck in the rocks, not able to
move . I eventually used a simple

`this value = new value `

and only updated the actual co-ordinates. This is the opposite in
principal to the JIGS game detection where the next oncoming pixel was
tested for boundary conditions, **before** making a move.

One after effect (at present at least )is that the screen will show a
value of black (r=0,G=0,B=0) but the spaceship won't actually have had
its coordinates updated, so it is still **in-bounds**,
