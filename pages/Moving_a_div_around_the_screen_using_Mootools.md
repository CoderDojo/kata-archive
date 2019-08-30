`This method will be used time and time again to move game elements around the screen. It comes in three stages`

  - Check The keypress.
  - Update coordinates.
  - Move the div.

\--Check The KeyPress --

`  `  
`    function check(e){`  
`        if (!e) var e = window.event;`  
`            (e.keyCode) ? key = e.keyCode : key = e.which;`  
`        try{`  
`            switch(key){`  
`                case 38: MoveUp(); `  
`                break;   `  
`                case 39: MoveRight(); `  
`                break; `  
`                case 40: MoveDown(); `  
`                break;`  
`                case 37: MoveLeft(); `  
`                break;      `  
`            }`  
`            `  
`        }catch(Exception){}`  
`    }`  
`  `  
` `

\--Increment or Decrement the position co-ordinates --

`  `  
`function MoveLeft(){`  
`                pX=pX-50;`  
`        Move_Player();`  
`        return;`  
`        }`  
`  `  
`function MoveRight(){`  
`                pX=pX+50;`  
`        Move_Player();`  
`        return ;`  
`        }`  
`function MoveUp(){`  
`                pY=pY-50;`  
`                Move_Player();`  
`        return;`  
`        }`  
`function MoveUp(){`  
`                pY=pY+50;`  
`                Move_Player();`  
`        return;`  
`        }`  
` `

\-- Finally Move the Div

`  `  
`function Move_Player(){ `  
`function(){ `  
`        var mover = new Fx.Move($('demo'), {`  
`        relativeTo: document.getElementById('screen_grid'),`  
`        position: 'upperLeft',`  
`        edge: 'upperLeft',`  
`      offset: {x: pX, y: pY}`  
`      });`  
`      `  
`     mover.start(); //moves to the new location`  
`      }`  
` `  
` `
