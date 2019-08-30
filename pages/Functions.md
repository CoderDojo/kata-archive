functions are ways of combining lines of related code to make it easier
to understand and maintain.

In this first example we choose between two different functions attack()
and adv\_attack.

`if ($choice =1) {`  
`attack();`  
`}`

`else `

`{`  
`adv_attack();`  
`}`

`attack(){`  
`  $player1_health = $player1_health -1;`  
`  return $player1_health;`  
`}`

`adv_attack{`  
`$player1_health = $player1_health - rand(0,6);`  
`  return $player1_health;`  
`}`

in this second example we tell the function who to attack

`if ($choice =1) {`  
`attack($player);`  
`}`

`else `

`{`  
`adv_attack($player);`  
`}`

`attack($player){`  
`  $player->health = $player->health -1;`  
`  $return $player;`  
`}`

`adv_attack($player)`  
`{`  
` $player->health = $player->health - rand(0,6);`  
` $return $player;`  
`}`

  - [Make a game](Tutorials_by_Galway.md)
