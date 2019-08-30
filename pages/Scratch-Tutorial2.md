## Summary

 How to make the background of your game move across the
screen, to give the impression that your sprites are moving quickly even
though they are remaining at the same “X” position on the screen.


## Tips for use

You will need to either install Scratch on the
[Ninja](Ninja.md)'s machine or use the [web-based
editor](https://scratch.mit.edu/) in advance of using these cards.

## Content

### How to do automatic horizontal background scrolling in Scratch

If you can make the background of your game move across the screen, it
will give the impression that your sprites are moving quickly even
though they are remaining at the same “X” position on the screen.

This tutorial will show you how to achieve this effect.

### Author

Thanks to Seamus Minogue for providing this tutorial

### Requirements for this tutorial

Extract (unzip) “scrolling tutorial.rar” into a directory of your
choice, this contains the graphics you need for this tutorial and the
same scratch project if you want to see it running straight away\! (See
link at bottom of this page)

  - Wall.gif
  - Mountains.gif
  - Background.gif

### To Begin

#### Step 1

  - Create a new project in Scratch
  - In the “New Sprite” section, click on “Paint new sprite”
  - Click on “Import” and select “wall.gif”.
  - Drag the graphic to the bottom of the edit window making sure to
    line the graphic up exactly with the bottom and left side of the
    window.

![Scratch1.PNG](../files/img/Scratch1.PNG "Scratch1.PNG")

  - Click on “Ok”
  - In the main scratch window, rename the sprite to “wall1”

![Scratch2.PNG](../files/img/Scratch2.PNG "Scratch2.PNG")

  - Add the following script to the “wall1” sprite

![Scratch3.PNG](../files/img/Scratch3.PNG "Scratch3.PNG")

**Note** The important thing here is the “y position”, at -150 this
moves this sprite to the bottom of the screen. If you have a larger
sprite, you will need to experiment with the “y position” until you get
it where you want it. Just make sure that the “y position” is set to the
same figure in the three highlighted areas of the picture above. It’s
always a good idea to set the start position of your sprites outside the
“forever” loop to make everything starts in the correct position.

The “glide” block above will determine the speed of the movement of the
background, so experiment with this until you get your the desired
speed.

  - Click on the “green flag” to start the game.

So what happens? Well, as expected, the wall scrolls to the left, but
wait\! Half of it is missing, what’s going on? This is the secret of
horizontal scrolling; you need **TWO** sprites to make the effect work.

#### Step 2

  - In the “New Sprite” section, click on “Paint new sprite”
  - Click on “Import” and select “wall.gif”.
  - As before drag the graphic to the bottom of the edit window making
    sure to line the graphic up exactly with the bottom and left side of
    the window.
  - Click on “Ok”.
  - Rename this sprite to “wall2”.
  - Add the following script block to sprite “wall2”

![Scratch4.PNG](../files/img/Scratch4.PNG "Scratch4.PNG")

  - Click on the “green flag” to run the game.

You should now see the wall scroll smoothly across the screen without
any gaps.

### Parallax Scrolling

Back in the day when your dad or mum was your age, we marvelled how
different backgrounds in video games moved at different speeds giving
the illusion of depth. This concept was called “parallax scrolling”.
Using the instruction above, we can reproduce this effect on scratch.

  - In the “New Sprite” section, click on “Paint new sprite”
  - Click on “Import” and select “mountains.gif”.
  - As before drag the graphic to the bottom of the edit window making
    sure to line the graphic up exactly with the bottom and left side of
    the window.
  - Click on “Ok”.
  - \!Rename this sprite to “mountains1”.
  - Add the following script block to sprite “mountains1”.

![Scratch5.PNG](../files/img/Scratch5.PNG "Scratch5.PNG")

  - Click on the “green flag” to start the game.

As you can see only half the mountains are scrolling but they are
scrolling slower than the wall, actually, it’s four times slower because
the “glide” block above is set to 40 seconds rather than 10 seconds for
the wall. You can experiment with this to get different speeds.

#### To add the rest of the mountain, take the following steps

  - In the “New Sprite” section, click on “Paint new sprite”
  - Click on “Import” and select “mountains.gif”.
  - As before drag the graphic to the bottom of the edit window making
    sure to line the graphic up exactly with the bottom and left side of
    the window.
  - Click on “Ok”.
  - Rename this sprite to “mountains2”.
  - Add the following script block to sprite “mountains2”.

![Scratch6.PNG](../files/img/Scratch6.PNG "Scratch6.PNG")

  - Click on the “Green flag” to start the game.

Now the mountains are scrolling smoothly across the screen.

#### To make the mountains stand out from the white background

  - click on the “Stage” button and then click on the “background”
    button and then the “Edit” button.
  - Click on “Import” and select “background.gif”.
  - Click on “Ok”.

Now those snow-capped mountains stand out really well\!

You can easily use your own graphics for your scrolling backgrounds but
to get the right effect, the left edge of your graphic should match up
with the right edge of your graphics so that they line up as one graphic
in scratch, with a little experimentation, you’ll get this right\!

### Downloads

  - A Rar (a file archive) containing scratch project and graphics
    at https://docs.google.com/open?id=0B7hSaTbVwfhDOGhmRVpNWmVRQWFDRkRsd2pLVC1Gdw
  - Link to the original tutorial document on Google Docs
    at https://docs.google.com/document/d/1LsZ2jnrbJtrpRRNQMqvf8qn2v\_itP\_wTKpeE8RIuIaA/edit
