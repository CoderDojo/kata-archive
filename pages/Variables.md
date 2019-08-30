variables are boxes of memory (think role playing stats)

`$player1_health   = 100 ;`  
`$player2_health   = 90 ;`  
`$player1_strength = 10;`  
`$player2_strength = 20;`  
`$player1_dice     = rand(0,6);`  
`$player2_dice     = rand(0,6);`

`if (player1_health + player1_dice > player2_health + player2_dice)`  
`{`  
`   player2_health = player2 health - 1;`  
`}`  
`else if `  
`if (player2_health + player2_dice > player1_health + player1_dice)`  
`{`  
`   player1_health = player1 health - 1;`  
`}`  
`else `  
`{`  
`echo "It's a draw";`  
`}`

  - [Return to Make a game](Tutorials_by_Galway.md)
