An object is a collection of strings, variables and functions belonging
to one entity, usually derived from a
class

`class ninja `  
`{`  
` $health = 100;`  
` $strength = 10`  
` function attack($enemy,$strength,$health)`  
` {`  
`     if ($enemy->strength > $strength)`  
`     {`  
`       health = health -10;`  
`       return $health;`  
`     }`  
`  }`  
`}`

`$red_ninja   = new ninja; // red_ninja is one object`  
`$black_ninja = new ninja; // black_ninja is one object`  
  
`// turn 1`  
`$red_ninja->attack($black_ninja);// red_ninja gets first go and attcks black_ninja`  
  
`// turn 2`  
`$black_ninja->attack($red_ninja);// black_ninja gets second go and attacks red_ninja`

  - [Make a game](Tutorials_by_Galway.md)
