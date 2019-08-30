## Javascript Call

``` Javascript numberLines
function punch(character_id){
  
 
    var d = document.getElementById('punch');
    var a = new Request.JSON({
            url: "index.php?option=com_battle&format=raw&task=action&action=attack&type=punch&character=" + character_id,
            onSuccess: function(result){

            text_message = (result[2] + ' me: ' + result[0].health + '   Him: ' + result[1].health);
            var new_message = new Element('p',{
            'display':'table-row',
            'html': text_message });
            
            new_message.inject('message_table','top');

                 npc_health = result[1].health;

                if (result[0].health <= 0 )  {
                    close();
                    jump();         
                    }
                if (result[1].health <= 0 ) {
                    close();
                    jump();
                    }       
                }
            }).get();
```

  - [Return to Make a game](Tutorials_by_Galway.md)
