Fractal Generation
The fractal generation works by starting with a number of points (in this explanation 1).
The algorithm then gives the parent point 4 "children" with horizontal locations 0,0 0,1 1,0 1,1
then the algorithm gives those points 4 more children making a grid of 16.
It repeats this as many times as the program specifies and then smooths the terrain.
The height of each child node is given by the parent's height * noise * the layer number
The layer number ensures that big changes happen in the higher layers and little fine changes in the lower layers.
The noise is just random.
