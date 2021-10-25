This is a simple python simulation code that uses neuro-evolution to learn how to run automated drone through obstacle

There are two python files included:

drone.py:

This is the genetic algorithm implementation for the idea.
This python file uses "index.png" image. Download this image if you are running the drone.py

Libraries used:

    pygame
    math
    random
    os
    numpy
    
Genetic Algorithm:

Basically, the idea is executed once with a certain number of drone (The Population). After this generation of the population finishes (i.e. every drone has crashed) the code will choose the best drone path(Choose the parameters upon which the it was deciding whether to jump or not jump). The best path will be choosen using a fitness equation which in this case is:
    
    Distance Travelled by the drone - (Distance between the center of the drone and the center of the gap between the pipes.

After the best drone parameters are selected, 10% of the drone in the next generation will be same as the drone bird of previous generation. The remaining 90% of the drone would be created using mutation.

The process repeats until and unless you get a near perfect bird, if not perfect.
