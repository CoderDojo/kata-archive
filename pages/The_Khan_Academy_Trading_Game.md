![trade.png](../files/img/trade.png "trade.png")

  - <https://www.khanacademy.org/cs/trade/1106707071>

This excellent tutorial can be extended in numerous ways. It has been
adapted to be downloaded and used with processsingJs. Add an armoury or
some new levels. This is an excellent introduction to single player
RPGS.

`from one student:`  
`When playing the base game, when you die in battle, it freezes. I added a very simple "game over" pop up:`  
`if(hp<0){`  
`println("Game Over");`

Downloadble version can be found here
[1](https://github.com/Techbot/template006)

  -   - At present I get a recursion error when I click the \[battle
        option\] . Any help appreciated. \*\*\*\*

Coverting a khan academy file to script.js

Step 1) replace all

var function\_name= function (){

with

void function\_name(){

for example

replace

var draw()=function(){

with

void draw(){

2\) replace mouseIspressed with mousepressed

3\) add the void setup() function as seen in template 4 and 6
