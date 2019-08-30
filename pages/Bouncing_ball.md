Not exactly a loop. Instead a function is called every ten milliseconds.
This uses mootools for the periodical call. We use mootools because it
comes with joomla. But it could just as easily be done with mootools and
even with raphael.

or what about making a proper game loop?

or even an animation loopthat takes into account
fps?

<script src =  "mootools-core.js">

</script>

<script src =  "mootools-more.js">

</script>

<script src =  "raphael-min.js">

</script>

</head>

<body style = "background:black;">

<d v id= "holder" style = "width:600px; height:480px; margin:0 auto; background:black;">

</div>

<d v id= "nav_cicles" style = "text-align:center;width:600px; margin: 0 auto; background:black;">

</div>

</body>

<script>

`var paper  =   Raphael('holder',600, 480);  `  
`var x      =   1;`  
`var y      =   12;`  
`var dirx   =   1;`  
`var diry   =   1;`  
`   `  
`function draw(){`  
`var circle = paper.circle(x, y, 10);`  
`circle.attr("fill", "#f00");`  
`circle.attr("stroke", "#fff");`  
`x = x + dirx;`  
`y= y + diry;`  
`if ( y == 460 || y== 0){`  
`  diry = -diry;`  
`}`  
`if ( x == 580|| x == 0){`  
`dirx = -dirx;`  
`}`  
`}`  
`draw.periodical(10);`
