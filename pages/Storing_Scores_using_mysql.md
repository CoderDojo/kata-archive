### Step 1 Gather stats

  - $query = "SELECT health,money,active FROM \#\_\_jigs\_players WHERE
    iduser = ".$user-\>id
  - $db-\>setQuery($query);
  - $result = $db-\>loadRow();
  - $player\_health = $result\[0\];
  - $player\_money = $result\[1\];
  - $player\_status = $result\[2\];

### Step 2 Adjust stats based on outcome

  - $player\_health = $player\_health -1;
  - $char\_health = $char\_health-30;
  - $player\_money = $player\_money + $char\_money ;

### Step 3 Save new stats to database

  - $db-\>setQuery("UPDATE \#\_\_jigs\_inventory SET
    \#\_\_jigs\_inventory.player\_id = " . $user-\>id . " WHERE
    \#\_\_jigs\_inventory.player\_id = " . $player\_id );
  - $result = $db-\>query();
  - $db-\>setQuery("UPDATE \#\_\_jigs\_players SET
    nbr\_kills=nbr\_kills+1, money = $player\_money WHERE
    \#\_\_jigs\_players.iduser = " . $user-\>id ) ;
