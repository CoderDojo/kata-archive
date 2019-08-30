Atthe top of each game you will find this code or an equivalent delta
time technique.

// requestAnim shim layer by Paul
Irish

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

This is then followed by something like

`   $( "#container" ).append( canvas );`  
`   `  
`   animate();`  
`   `  
`   function animate() {`  
`   requestAnimFrame( animate );`  
`   draw();`  
`   }`

You don't really need to know what is going on, but know
this

`   function draw()`  
`   {`  
`   // this is your entry point. This function will be called between 30 and 60 times a second depending on your browser.`  
`   }`

Of course you can call other functions from within draw(), but draw() IS
your [game loop](game_loop.md)

It will adjust to your browser ensure a consistant game , and it will
even pause if you jump to another browser tab. It might feel a bit
clunky, all those different browser calls. But knowing that draw() is
your entry point is just so cool.

I'll explain some other delta time techniques next.
