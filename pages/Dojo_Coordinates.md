To find out the coordinates of you Dojo,

goto [Google Maps](http://maps.google.com), find the location of your
Dojo on it and copy and paste the Javascript snipper below into your URL
bar:

javascript:void(prompt('',gApplication.getMap().getCenter()));

Up pops the coordinates of the centered location. You can verify this by
pasting the coordinates into the Google Maps search bar, if correct, a
pin with pop up on the Dojo's location.

If using the coordinates on Zen, make sure you remove the brackets on
either side of the coordinates you get from the prompt first though\!
(correct: *-xx.xxx, xx.xxxx*, incorrect: *(-xx.xxxx, xx.xxxxx)* )

![Coordinates\_gmaps\_demo.png](../files/img/Coordinates_gmaps_demo.png
"Coordinates_gmaps_demo.png")
