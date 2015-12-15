# Final exam for CST 112

#### Begin with a copy of your "Project-9" code, <BR> then add the following new features to it:
1. Draw an evenly-spaced set of __red triangles__, underwater, from surface to bottom, along the right side of the screen.    See http://suffolk.li/cst112/59cst112/day/bam//Screen_Shot_2015-12-13_at_6.35.34_PM.png

2. Do __not__ assume the screen size is constant.  
  All features and movements should adjust to the size of the screen, the position of the surface, etc.  
  *(Avoid constant values, and use `height` and `width`!)*

3. Create a new object class **`Lobster`**, with properties and methods to accomplish following:
  * Show a creature with two animated "claws" that open and close as it moves.  
    _Claws should face forward, in the direction of motion_.
   See http://suffolk.li/cst112/59cst112/day/bam//Screen_Shot_2015-12-13_at_7.15.31_PM.png
  * Use a constructor to initialize properties of each "Lobster" to:
    * start on the left side, at a random height in the lower half of the water, 
    * move to the right with a random horizontal speed (dx > 0), and
    * move upward with a random speed (dy < 0).
  * Bounce off the surface and bottom (reversing dy) and bounce off the sides (reversing dx).  
    _You may re-use old code from pool-table Ball objects._
  * Also include a **`hit( x, y )`** method, to return `true` iff this Lobster is near the coordinates (x,y).

3. Make an array of **`Lobster`** objects, using YOUR OWN initials.  
   _If your name is Donald Trump, then your array should be declared as:_  **`Lobster[] dt`** 

5. Add code to make all of the "Lobsters" move and show themselves.

6. Add code to make any **`Squid`** object go to the bottom, when a **`Lobster`** hits (gets near) it. 

5. Add a __report__ for the array of **`Lobster`** objects.  
    _(Sorting is NOT required for this exam.)_

6. Add a __"LEFT-RIGHT"__ button, and display the (x,y) positions of the leftmost and rightmost crabs (i.e. the two crabs with the highest and lowest X coordinate value), whever this button is clicked or the '$' key is pressed.

Readability and good coding practices are important:
- Before each new function you write, there should be a comment line stating its __purpose__.  
- Points will be deducted for uncommented functions, meaningless variable names, lack of modularization, inconsistent indentation within code blocks, and other poor software practices that impair readability of code.  
- Points will be added for very good readability of code.

___
#### NOTE:  To be graded, your final exam must meet ALL of the following conditions:
- Your code must be in a file named **`final-xyz.java`** _(where_ **`xyz`** _is your own initials_).
- This code file must be in a repository named **`Final`** forked from http://github.com/bam59cst112day/Final
- This repository must be in your Github.com account on http://github.com
- Your code must __compile__ and __run__ *(in the Processing PDE)*
- Your name should __appear__ on the screen (in the lower-left corner).
- Your full __name__ must appear within the first few lines of the file *(in a comment line or String)*

**Code that fails to meet ALL of the above conditions will NOT be considered.**
___
Similar conditions apply to your **`project9.java`** file,  
within a **`project9`** repository in your Github account  
_(forked from [http://github.com/bam59cst112day/project9](https://github.com/bam59cst112day/project9/blob/master/README.md) )_.  
Project9 uses loops to manipulate an array of **`Squid`** objects and an array of **`Boat`** objects,
then displays a "report" listing the properties of each object.
