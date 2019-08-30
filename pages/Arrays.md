Arrays are
lists

`$message[0] = " You are standing in a room";`  
`$message[1] = " You climb the wall";`

`if $input = "climb" {`  
`echo $message[1];`  
`}`

or

`$inventory = array("key", "gun", "torch", "sword");`

`if (in_array("torch",$inventory))`  
`{`  
`   echo "You can see in the dark";`  
`}`

or

`$inventory = array("key", "gun", "torch", "sword");`

`echo "Your third object is a " . $inventory[2]; // remember we start with [0]`

  - [Make a game](Tutorials_by_Galway.md)
