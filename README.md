                                        Awesome Ray Tracing 
                                        -------------------

Observer observes viewport.

                      Viewport
                        
                    - [l, n, p]
                -   
    Observer -------- [o, k, a]      
                -                    
                    - [q, b, h]     



    Our viewport [ l , n , p ] is a 3X3 set of pixels which can display on your screen!
                 [ o , k , a ]
                 [ q , b , h ]


The viewport here exists here in our 3D cartesian plane.

                                a 3D cartesian plane is a 3D matrix of points X, Y, Z.
                                             |
                                             |
                                             V
       .+------+     +------+     +------+     +------+     +------+.
     .' |    .'|    /|     /|     |      |     |\     |\    |`.    | `.
    +---+--+'  |   +-+----+ |     +------+     | +----+-+   |  `+--+---+
    |   |  |   |   | |    | |     |      |     | |    | |   |   |  |   |
    |  ,+--+---+   | +----+-+     +------+     +-+----+ |   +---+--+   |
    |.'    | .'    |/     |/      |      |      \|     \|    `. |   `. |
    +------+'      +------+       +------+       +------+      `+------+
                      

X, Y, Z represent every possible ray location in our 3D cartesian plane.


          ;   :   ;
       .   \_,!,_/   ,
        `.,'     `.,'          Light rays fired in all directions like the sun!
         /         \               Light exists in our 3D cartesian plane. 
    ~ -- : The Sun  : -- ~  
         \         /
        ,'`._   _.'`.
       '   / `!` \   `
          ;   :   ;  


Updated 3D cartesian plane

                 .+----------------------------------+
               .' |                                .'|
              +---+------------------------------+'  |
              |   |  \ | /                       |   |
              |   |--- O ---                     |   |
              |   |  / | \                       |   |          Updated 3D cartesian plane
              |   |                              |   |             + Add light source 
              |   |       [l,n,p]                |   |             + Add viewport
              |   |       [o,k,a]                |   |
              |   |       [q,b,h]                |   |
              |  ,+------------------------------+---+
              |.'                                | .'
              +----------------------------------+'


Rays bounce in 3D cartesian plane and hit viewport.

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


Viewport performs calculation using ray direction and ray data to renders
the viewport.

                                                  Viewport
                                                    
                                                - [l, n, p]
                                            -   
                            \( ﾟヮﾟ)/     -------- [o, k, a] 
                            Observer        -   
                                                - [q, b, h]     





---

Thank you for reading.

Have a wonderful day.
