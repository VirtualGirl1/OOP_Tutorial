# Activity

To demonstrate the concepts you learned in the previous section 
here is a small activity to create a simple class library for a home 
renovation system.

Your library will implement the following classes

![](RenoSys.jpg)

`ToString()` must return all set properties in class as a comma separated list

## Opening class 

Rules:
 - Edging must be <= 0
 - Opening type must be:
   - Door
   - Window
   - Closet

The constructor takes the following arguments:
 - Type
 - width
 - height
 - edging

## Wall class

Rules:
 - if an opening is given it cannot cover more than 80% of the wall
   - Divide Opening.Area by Wall.SurfaceArea and multiply by 100 to get the percent

The constructor takes the following arguments:
 - Color
 - width
 - height
 - opening


## Room class

Rules:
 - A room must have at least 4 walls
 - One of these walls must have a door
 - flooring cannot be an empty string
 - Name cannot be an empty string

The constructor takes the following arguments:
 - Name 
 - flooring
 - Walls

