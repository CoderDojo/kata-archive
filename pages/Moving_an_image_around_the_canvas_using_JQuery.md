  - [Back to make a game](Tutorials_by_Galway.md)

# How to make a platform game

The game is pretty simple with no collsion detection, no baddies, no
scrolling, but a game loop powered by requestanimationframe. When a key
is pressed, it is detected by jquery , the background image object and
the character are moved in opposite directions. When the up key is
pressed the player will jump until a maximum height is reached, and will
begin the decend function at this point or if the up button is released
before the maximum height is reached.

![platform001.png](../files/img/platform001.png "platform001.png")

  - Step 1: Setup the Global variables
  - Step 2: Call init once to init the canvas
  - Step 3: use animate (and request animframe) to call the draw()
    function based on the frames per second returned by the browser.
    This means that you don't need to worry abot one computer being
    faster than another.
  - Step 4: Add new functions to be called from draw().

It also means you only need to focus on the draw() function, this is the
game loop where everything happens. You could, of course, have more
functions being called from within draw(). but essentially as long as it
is inside the draw() function, the browser will continually execute it.
And if you change to another tab, the game is automatically paused.
Neat\!

`//Global Variables can be accessed from inside or outside of any function or method, `  
`//they are generally frowned upon but are used a lot in games.`  
`var  canvas, context, toggle;`  
`var y= 0;`  
`var x= 0;`  
`var dirX =1;`  
`var dirY =1;`  
`var destX  ;`  
`var destY ;`  
`var i;`  
`var state ;`  
`var status = -1; // -1: stopped  , 0 In play   `  
`var imageObj = new Image();    `  
`var background_obj= new Image();`  
`var jump = 'rest';`  
`var backg_x = 0;`  
`var backg_y = 0;`  
`background_obj.src = "level_bounds.png";`  
`imageObj.src = "fnord.png";`

/////////////////////////////////////////

`init();`  
`animate();`

/////////////////////////////////////////

`function init() {`  
`   canvas = document.createElement( 'canvas' );`  
`   canvas.width = 568;`  
`   canvas.height = 300;`  
`   context = canvas.getContext( '2d' );`  
`      `  
`  $( "#container" ).append( canvas );`  
`}`

////////////////////////////////////////

`function animate() {`  
`   requestAnimFrame( animate );`  
`   draw();`  
`}`

////////////////////////////////////////

`function draw() {`  
`context.fillText( state + ":" , canvas.width / 2 , canvas.height / 2 );`  
`$(document).keyup(function(e) {`  
`if (e.keyCode == 37){`  
`state= "stop";`  
`}`  
`if (e.keyCode == 39){`  
`state= "stop";`  
`}`  
`if (e.keyCode == 38){`  
`jump = 'descend';`  
`}`  
`});`  
`///////////////////////`  
`//`  
`// Jquery test for keypress`  
`//`  
`///////////////////////`  
`$(document).keydown(function(e) {`  
`// alert (e.keyCode);`  
`// if space start/stop gameloop`  
`if(e.keyCode == 32){`  
`status = 0 - status;`  
`}`  
`// Only allow a jump keypress if the player is not already in the middle of a jump`  
`if (jump != 'descend'){`  
`if (e.keyCode == 38 ){`  
`jump = 'ascend';`  
`}`  
`}`  
`// Not used in game yet`  
`if (e.keyCode == 40){`  
`// down`  
`}`  
`// If Keypress is left arrow`  
` if (e.keyCode == 37){`  
` state = 'left'; // we set a state instead of executing the code here,so that an object might continue moving after key is pressed or released`  
` }`  
`// If Keypress is right arrow`  
` if (e.keyCode == 39){`  
`state = 'right';`  
`}`  
`});`

//////////////////////////////

`if (state == 'left') {`  
`x = x-(1 * dirX);`  
`backg_x = backg_x + 1 ;`  
` }`  
`if (state == 'right') {`  
`x      = x + (1 * dirX);`  
`backg_x = backg_x - 1 ;`  
`}`  
`if (jump == 'ascend'){`  
`y = y-1;`  
`if (y <= -40){`  
`jump = 'descend';`  
`}`  
`}`  
`if (jump == 'descend'){`  
`y=y+1;`  
`if (y >= 0){`  
`jump = 'rest';`  
`}`  
`}`  
`if (jump == 'rest')`  
`{`  
`y = 0;`  
`dirY = -1;`  
`}`  
`// Set the co-ordinates based on centre of screen plus new x and y`  
`destX = (canvas.width / 2 ) + x;`  
`destY = (canvas.height / 2 ) + y;`  
  
`// Hit the edge of canvas`  
`if (destX > canvas.width || destX < 0)`  
`{`  
`dirX=-dirX;`  
`}`  
`if (destY > canvas.width || destY < 0)`  
`{`  
`dirY=-dirY;`  
`}`  
`// Finally clear the screen and redraw objects`  
`context.clearRect(0,0 , canvas.width, canvas.height);`  
`context.drawImage(background_obj, backg_x, backg_y);`  
`context.drawImage(imageObj, destX, destY);`  
`}`

//////////////////////////////////////////////////////////////////////////////

`// requestAnim shim layer by Paul Irish`  
`   window.requestAnimFrame = (function(){`  
`     return  window.requestAnimationFrame       || `  
`             window.webkitRequestAnimationFrame || `  
`             window.mozRequestAnimationFrame    || `  
`             window.oRequestAnimationFrame      || `  
`             window.msRequestAnimationFrame     || `  
`             function(/* function */ callback, /* DOMElement */ element){`  
`               window.setTimeout(callback, 1000 / 60);`  
`             };`  
`   })();`  
`// example code from mr doob : `<http://mrdoob.com/lab/javascript/requestanimationframe/>

//////////////////////////////////////////////////////////////////////////////
