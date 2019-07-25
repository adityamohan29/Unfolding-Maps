# Unfolding-Maps
Final assignment of the Coursera course of Object Oriented Programming in Java by the University of California, San Diego. The course progresses with a hands on exprience of developing an interactive map using the Unfolding Maps and Processing libraries. The map contained markers pertaining to a few earthquakes along with some of its features like magnitude and threat circle to name a few. It helped us in developing multiple functionalities and GUIs like responding to mouse click and hovers and making a key for representing the symbols used.

I've added only the classes which were relevant to my final extension.

My extended functionality:-

When the earthquake button is clicked, it shows a relative threat circle perimeter. Since, the threat circle is obtained in kilometers, I have taken a relative measure which is shown on the screen. On the output screen, an earthquake which occurred elsewhere with a similar magnitude to the one which is clicked on is displayed.

The way I did it was:-

1. I changed the Threat Circle variable to a static variable which enabled me to use the variable in a different class. This led me to draw an ellipse whenever the mouse position is clicked within the boundaries of the earthquake markers. The size of the ellipse was the relative size of the threat circle.
2. The quakes list which was sorted in the sortAndPrint function was used to identify the quakes which have occurred with the same magnitude by simply comparing the magnitude of the selected quakes with the neighboring ones in the list.
