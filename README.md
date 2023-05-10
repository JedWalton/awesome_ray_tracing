                                        TLDR Ray Tracing 
                                        ----------------
---
We have a viewport.

                      Viewport
                        
                    - [l, n, p]
                -   
     (⌐■_■)  -------- [o, k, a]      
    Observer    -                    
                    - [q, b, h]     


    Viewport is a 3X3 set of pixels which can display on your screen!
                - It can be any resolution e.g. 1920x1080

---
We have a 3D cartesian plane.

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
                      
---
We have a light source.

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
Put light source and viewport in plane.

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
Fire rays from light source.

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
Observe ray traced output in viewport.


                                     Viewport
             Aww yeah                          
                  \                - [l, n, p]     - Viewport output calculated using ray data.
                   \            -                  - Viewport output is rendered. 
                    (⌐■_■)  -------- [o, k, a]      
                   Observer    -                    
                                   - [q, b, h]     


---

Thanks for reading.
