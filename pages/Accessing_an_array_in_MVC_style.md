This object of this tutorial is to present 3 concepts

  - MVC (Model-View-Controller)
  - Arrays
  - The Foreach loop

\-- The View --

view.html.php

`  `  
`  `  
` <?php defined( '_JEXEC' ) or die( 'Restricted access' );`  
`  `  
`jimport( 'joomla.application.component.view');`  
`  `  
`class CapitalsViewQuiz extends JView`  
`{   `  
`    function display($tpl = null)`  
`    {`  
`        $model = &$this->getModel();`  
`        $capitals = $model->get_capitals();`  
`        $this->assignRef('capitals',$capitals);`  
`        parent::display($tpl);`  
`    }`  
`}`  
` `

\-- The Views template--

`  `  
`  `  
`<?php defined( '_JEXEC' ) or die( 'Restricted access' ); `  
`jimport( 'joomla.methods' ); `  
`  `  
`foreach($this->capitals as $key => $row){`  
`echo $key .  " is capital of " . $row . "</br>";`  
` }`  
`  `  
`?>`  
`  `  
` `

\-- The Model --

`  `  
`<?php`  
`defined( '_JEXEC' ) or die( 'Restricted access' );`  
`  `  
`jimport('joomla.application.component.model');`  
`  `  
`class CapitalsModelQuiz extends JModel {`  
`    `  
`    function get_capitals(){`  
`  `  
`        $array = array(`  
`        "Dublin" => "Ireland",`  
`        "London"  => "England",`  
`        "Canberra" => "Australia",`  
`        "Budapest"=> "Hungary"`  
`    );`  
`        return ($array);`  
`    }`  
`}`  
` `
