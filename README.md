### Ray Tracing made awesome!

A 3D "map" or vector space is a series of coordinates. X, Y, Z

Observer looks at a viewport.


                - [l, n, p]
            -   
Observer -------- [o, k, a]      Over here is our 3D cartesian plane.
            -                       The rays in our model are traced from the
                - [q, b, h]         light in our 3D cartesian plane and reflect 
                                    around of different surfaces.

                                    These rays will hit the view port and 
                                    display on screen :)


Our viewport [l,n,p] is a 3X3 set of pixels which can display on your screen!
             [o,k,a]
             [q,b,h]


The viewport here exists as a set of coordinates in our 3D cartesian plane.

                        Viewport exists is our 3D cartesian plane.
                            a 3D cartesian plane is just 3D matrix.
                            X, Y, Z.     |
                                         |
                                         V
   .+------+     +------+     +------+     +------+     +------+.
 .' |    .'|    /|     /|     |      |     |\     |\    |`.    | `.
+---+--+'  |   +-+----+ |     +------+     | +----+-+   |  `+--+---+
|   |  |   |   | |    | |     |      |     | |    | |   |   |  |   |
|  ,+--+---+   | +----+-+     +------+     +-+----+ |   +---+--+   |
|.'    | .'    |/     |/      |      |      \|     \|    `. |   `. |
+------+'      +------+       +------+       +------+      `+------+
                        

A 3D map can be represented by coordinates. X, Y, Z.

X, Y, Z represent every possible place a light ray could be in our 3D cartesian
plane.

We can create a light source in our 3D vector space. This light source will 
fire rays in all directions like the sun!


          ;   :   ;
       .   \_,!,_/   ,
        `.,'     `.,'          Light rays fired in all directions!
         /         \               Sun exists in our 3D cartesian plane. 
    ~ -- : The Sun  : -- ~  
         \         /
        ,'`._   _.'`.
       '   / `!` \   `
          ;   :   ;  


 Here's our update cartesian plane! 

                 .+----------------------------------+
               .' |                                .'|
              +---+------------------------------+'  |
              |   |  \ | /                       |   |
              |   |--- O ---                     |   |
              |   |  / | \                       |   |
              |   |                              |   |
              |   |       [l,n,p]                |   |
              |   |       [o,k,a]                |   |
              |   |       [q,b,h]                |   |
              |  ,+------------------------------+---+
              |.'                                | .'
              +----------------------------------+'


The suns rays bounce around the 3D cartesian plane and eventually hit our
viewport!

This shows the light from the sun 'Ray Traced'
around our lovely 3D cartesian plane to hit the viewport!


                         .+----------------------------------+
                       .' |                                .'|
                      +---+------------------------------+'  |
                      |   |  \ | / \                     |   |
                      |   |--- O ---\                    |   |
                      |   |  / | \   \                   |   |
                      |   | /     \   \                  |   |
                      |   |/      [l,n,p]                |   |
                      |   |\      [o,k,a]                |   |
                      |   | \    /[q,b,h]                |   |
                      |  ,+--\--/-----------------------+---+
                      |.'     \/                         | .'
                      +----------------------------------+'


Here we see a ray reaching l, p and o in our viewport matrix! :)

Now, a simple calculation is needed to find the angle and direction of our ray
which can then be used to light up our viewport!


                             \( ﾟヮﾟ)/

