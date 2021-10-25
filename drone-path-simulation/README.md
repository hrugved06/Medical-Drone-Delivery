# Drone-Simulation
This is a simple python code that uses neuro-evolution to learn how to avoid obstacle by drone

There are two python files included:

Game.py:

This is a simple game that can be played raw using the "space" key to jump.
It will use the "index2.png" file. Download the image and keep it in the same folder as Game.py

drone.py:

This is the genetic algorithm implementation for the drone.
This python file uses "index.png" image. Download this image if you are running the drone.py

Libraries used:

    pygame
    math
    random
    os
    numpy
    
Genetic Algorithm:

Basically, the game is executed once with a certain number of drone (The Population). After this generation of the population finishes playing the game(i.e. every drone has lost) the code will choose the best drone(Choose the parameters upon which the it was deciding whether to jump or not jump). The best drone will be choosen using a fitness equation which in this case is:
    
    Distance Travelled by the drone - (Distance between the center of the drone and the center of the gap between the pipes.

After the best drone parameters are selected, 10% of the drone in the next generation will be same as the best drone of previous generation. The remaining 90% of the drone would be created using mutation.

The process repeats until and unless you get a near perfect drone, if not perfect.
