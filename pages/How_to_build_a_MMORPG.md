## MMORPG

  - [Return to Dojogame](Dojogame.md)

The complete code for this MMORPG server system is available at github
<https://github.com/Techbot/JiGS> JiGS is a fully functional MMORPG
written by CoderDojo mentors . It contains numerous "chapters" made by
the students over the past year, as well as a trading system, a chat
sytem, an economy which includes mining, trading, energy generation and
manufacture. It is built in php,javscript and mysql and uses the Joomla
CMS to manage story lines, user registration, security and plugin
framework .

## Introduction

  - [How to build a MMORPG -The legend of Tim the Ninja
    ](How_to_build_a_MMORPG.md)- From Galway Dojo \#1,4. Credit:
    [Techbot](User:Techbot.md)

JiGS is a fully functional MMORPG written by coderdojo mentors . It
contains numerous "chapters" made by the students over the past year, as
well as a trading system, a chat sytem, an economy which includes
mining, trading, energy generation and manufacture.

It is built in php,javscript and mysql and uses the Joomla CMS to manage
story lines, user regsitration, security and plugin framework . ![
200px|left](../files/img/15_Map.jpg " 200px|left") The game is extendable by using
plugins. It is up to mentor and advanced students to build plugins that
will allow each server evolve in it's own unique way, solving particular
problems per server from pure gaming to questions on fuel use and the
environment crime etc.

Rather than being an otheright MASSIVE morpg , JiGS is more a MEDIUM
morpg suiting an average of around 100 players who compete or
collaborate to rule the area. So one website per dojo might be suitable.

The Legend of Tim the Ninja is coderdojo galways instance of the game.
The idea is: Once student has built the simple game using html, he/she
then converts it to php simply by renaming the files (and installing
Xampp). Once this is done we begin the process of refectoring the code
to make use of the Jigs system.

## Features

  - When a player finishes one student's "chapter", he/she wins money
    that can be used in a different students "chapter".

<!-- end list -->

  - Each students chapter can be unique with it's own coding style

<!-- end list -->

  - Each chapter can be plugged into the larger game regardless of the
    students skill level.

<!-- end list -->

  - The more skilled the student, the tighter the integration with the
    main engine.

<!-- end list -->

  - The more skilled the student the more varied the chapter can be
    leading up to platform and arcade games.

<!-- end list -->

  - Student collaboration means richer more involved game design.

<!-- end list -->

  - Extremely low (test proven) entry point, grabs a students attention
    in the first 30 minutes.

<!-- end list -->

  - Infinitely customisable and extendable.

## Why Joomla\! as a games framework

The games we have been building to date are single player games and thus
html5's javscript and Css3 are fine for keeping scores etc. But once we
begin dealing with multiplayer games then the **validation must be done
server side**. and this is where Php comes in.

We could of course use node.js or one of the other serverside scripts.
But using php and in particular the Joomla framework we will be able to
use code already builtin, that will look after user management, security
and certain interactions with the browser via mootools. With the new
Joomla platform (an offshoot of the joomla CMS) we can run things from
the command line adding a new dimension to php game scripting.

While Joomla is a content management sytem and application development
platform, it was never designed to be a games framework, however recent
advances in joomla development has introduced joomla into territories it
was not orignally designed for . It is in this spirit we will use it to
create a game engine. where others will use our system to create games
we never imagined.

Joomla will
provide:

`a) An API for extending the game with components,modules,plugins and templates`  
`b) A user managment system that includes registration, login, player profile and extendability eg scores and player stats.`  
`c) A set of methods to communitcater with the browser via javascripts JSON and websockets.`  
`d) An MVC structure (the defacto architecture for modern software design).`  
`e) A library management system for introducing new functionality eg javascript libraries, libraries for exporting to pdf and of course our game libraries.`  
`f) A framework that is used in the real world. Joomla is not a games library it is one of the most popoular open source web system and mastering it will not only enable you to create games, it will provide you with the skills to create media rich websites and web applications.`

By following these series of projects you will master:
Php,HTML5,Mysql,Javascript,JSON,XML

## JiGS, Zen and Art Of The Dojo Game

  - [Tutorials\_on\_Joomla\!](Tutorials_on_Joomla!.md)- From
    Galway Dojo \#2,2. Credit: Techbot
  - [Why Joomla as a games
    framework](Why_Joomla_as_a_games_framework-.md) - From
    Galway Dojo. Credit: [Techbot](User:Techbot.md)
  - [The Yin and Yang of Dojo
    Game](The_Yin_and_Yang_of_Dojo_Game.md)- From Galway Dojo
    \#2,1. Credit: [Techbot](User:Techbot.md)
