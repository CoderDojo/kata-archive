# Summary

 So you think you know everything there is to know in
Scratch? Are you ready for a real challenge? Time to build what can be
the most complex genre of old-style computer games… 

## Tips for use

You will need to either install Scratch on the
[Ninja](Ninja.md)'s machine or use the [web-based
editor](https://scratch.mit.edu/) in advance of using these cards.

## Project

### **Dungeon Quest\!**

Back to [ScratchTastic](ScratchTastic.md)

You are a brave adventurer looking for danger and you will find it the
ancient dungeons of Moria.

Sneaky traps, fiendish puzzles, aggressive enemies and mountains of
treasure await…only if you are brave enough…

Use your Scratch skills to build the ultimate adventure game.

So how do these type of games work?

Basically, the dungeon is a grid and each square on the grid is 32
pixels by 32 pixels and each sprite in the game is also 32 pixels by 32
pixels, so imagine a chess board or a draughts board where the pieces
have to be placed in a specific square and you get the idea.

The part of the dungeon you can walk through is the path and this is
made up of squares placed on the grid. The adventure can only walk on
this path and so can the enemies and items can be found on the path. The
other squares on the grid can be made up of walls, water or even lava\!
Obviously your adventurer can’t walk through walls (a level 60 mage
probably could but that’s for another day) and what you want to happen
when your adventurer stumbles into water or lava, I’ll leave that up to
you…

An example of a dungeon path, you enter on the left and leave it on the
right, if you are lucky…

This works well if you create an image of 960 pixels by 720 pixels and
use this as your stage. If you create multiple paths, you can add them
as different costumes on the stage.

Notice that the walls are edged with white. The stops our adventurer
from walking into the walls. Simply use the “touching colour block”. As
you probably know by now, using this approach will prevent you from
using white elsewhere in the game so remember to replace white in your
sprites with a slightly different shade of white in your game.

I recommend downloading Paint.Net <http://www.getpaint.net/> . It’s free
and great for manipulating graphics. With all due respect to the makers
of Scratch, the sprite editor is pretty rubbish.

Because the game is based on a grid, the movement of our adventure is
controlled by the grid. He/she can move in four directions
(up/down/left/right) and if you map those directions to the arrow keys,
the adventurer sprite should move 32 pixels in whatever direction you
choose when you press a key. Each time you press a key, you will need to
check to see if you can move your character, if you touch a white wall
move the adventurer back to his/her original position, to do this you
will need to store the adventurer’s current X and Y position before you
move the sprite. That way, you can move the sprite back if you touch a
wall.

So what else can you do?

Be creative, create traps such as collapsible floors, arrows coming out
of walls etc. Look at ways of disabling those traps. Find keys for
hidden treasure chests, unlock doors to new parts of the dungeon. Raise
a drawbridge to cross streams of lava or water. Lock monsters into
rooms.

Did I say monsters?

Orcs, trolls, one-eyed floating balls of evil, gigantic spiders,
skeletons are known to inhabit these dark places and it’s clear them and
steal their treasure\!

How do I fight them?

I’m sure most of you have played some sort of role-playing game on a
games console or a PC at this stage but in case you haven’t…

You adventurer should have the following characteristics:

  - **Health** – Full health is 100, Dead is zero, loss health when you
    are hurt in fights, traps etc, regain health by eating food.

<!-- end list -->

  - **Strength** – How strong you are, how much you can carry. (0-5
    weak, 6-10 average, 11-15 strong)

<!-- end list -->

  - **Attack** – How much damage you do to enemies when you hurt, this
    reduces there health and they die when it reaches zero. The dungeon
    is littered with ancient powerful weapons that will add to your
    attach capabilities. Start at 1 and build up from there.

<!-- end list -->

  - **Defence** – You can prevent losing health by having a good
    defence, wearing armour that you find in the dungeon may help. Start
    at 1 and build up from there.

How complex you want to make the above is up to you, a word of advice,
start simple get it working and build up from there.

If you are feeling brave, you could add the characteristic of experience
(XP) which you gain when you defeat enemies, unlock doors/treasure
chests and defeat traps. When you get to 100 XP, you can “level-up”
which gives you the opportunity to add points to
health/strength/attach/defence. Remember to make your enemies
tougher/smarter as you gain levels.

Another area that you should try and implement is an “inventory” which
is basically all the weapons, food, keys etc that you will pick on your
adventure. Use the “lists” block in Scratch to accomplish this. You
might want to pick up something but not use it straight away, you might
need it later…

Try and make your enemies somewhat smart, get them to walk automatically
around a room in the dungeon, that way it would be harder for you to
sneak past you. Maybe get them to fire arrows/fireballs/spells at you
from a distance (these would need to be stopped by walls to of
course\!).

Of course, it’s not going to be much of a game if you know where all the
good stuff is to try to devise a way that you don’t see that
key/food/weapon until you are standing right beside them (use the
“Distance To” block and set a variable to determine how close you need
to be to see things). The same concept can also be used to prevent
enemies from seeing you until you are close to them. Try and see if you
can come up with a way of giving these items a random position each time
you play the game.

Try adding a few magic potions that will give your adventurer a
temporary “power-up” or restore full health (useful for dealing with
that dragon that might be lurking around

somewhere…)

When you are making the game, get other people to test it for you
(family/friends etc), what works fine for you may not work for them,
also its great fun watching them fall for

your devious traps…

We’ll give you a bunch of graphics to help you on your way but feel to
create your own.

This project will really stretch your Scratch skills so take your time
and try and implement one thing at a time, test it and try to come up
with ways or breaking it.

If you are interested in giving it a go, let me know and I’ll give you
the files you need and we’ll see you back in September and see how
you’ve got on…

… will you survive the…

Dungeons of Moria?
