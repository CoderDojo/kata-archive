  - [Make a game](Tutorials_by_Galway.md)

## index.php

create a url with your stats

  - \<a href ="index2.php?player=2\&health=90\&strength=99\> attack
    monster </a>

## index2.php

  - $responses = $\_REQUEST;

<!-- end list -->

  - $player\_id = $response\['id'\];

<!-- end list -->

  - $player\_health = $response\['health'\];

<!-- end list -->

  - $player\_strength = $response\['strength'\];

<!-- end list -->

  - echo "player id : " . $player\_id . "</br>";

<!-- end list -->

  - echo "player health : " . $player\_health . "</br>";
