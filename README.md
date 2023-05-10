                                        Awesome Ray Tracing 
                                        -------------------

                TLDR ray tracing  

Observer observes viewport.

                      Viewport
                        
                    - [l, n, p]
                -   
     (⌐■_■)  -------- [o, k, a]      
    Observer    -                    
                    - [q, b, h]     



    Our viewport [ l , n , p ] is a 3X3 set of pixels which can display on your screen!
                 [ o , k , a ]
                 [ q , b , h ]


The viewport exists in our 3D cartesian plane.

                      3D cartesian plane is a 3D matrix of coordinaties X, Y, Z.
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
                      


          ;   :   ;
       .   \_,!,_/   ,
        `.,'     `.,'              - Like the Sun, Light rays are fired in all directions.
         /         \               - Light exists in our 3D cartesian plane. 
    ~ -- : The Sun  : -- ~  
         \         /
        ,'`._   _.'`.
       '   / `!` \   `
          ;   :   ;  

---

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

---

                .+----------------------------------+
              .' |                                .'|
             +---+------------------------------+'  |
             |   |  \ | / \                     |   |          - Rays fired in all directions.
             |   |--- O ---\                    |   |          - Rays bounce around until they 
             |   |  / | \   \                   |   |             hit the viewport.
             |   | /     \   \                  |   |
             |   |/      [l,n,p]                |   |
             |   |\      [o,k,a]                |   |
             |   | \    /[q,b,h]                |   |
             |  ,+--\--/-----------------------+---+
             |.'     \/                         | .'
             +----------------------------------+'

---



                                     Viewport
             Aww yeah                          
                  \                - [l, n, p]     - Viewport output calculated using ray data.
                   \            -                  - Viewport output is rendered. 
                    (⌐■_■)  -------- [o, k, a]      
                   Observer    -                    
                                   - [q, b, h]     


---

Thanks for reading.
