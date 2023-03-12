# GUI pathfinding project
This project is wrote in python using pygame to make a Graphic User Interface. This GUI give the possibility to the user to make his own map, where are the start, end and the walls. There is a "random map" button which will randomize the map if the user doesn't want to make his own. Once the user choosed the disposition of the map, he can run the algorithms and see the difference in time complexity it take for Djikstra and a A* to reach the end.

# The difference between A star and Djikstra

A star is a pathfinding algorithm using heuristic, it means it take in count where is the end, so it will aim to explore the tiles in the direction of the end.
Djikstra doesn't use heuristic, it will just explore every tiles which are next to the ones already treated.
The main advantage of A star over Djikstra is the time complexity is smaller by quite a margin. 
It means Djikstra will take more time to found a path than A star.
However, Djikstra doesn't need to know here is the end, so if we need to find a path without knowing where to go, we can't use A star but we can use Djikstra.


# When you start running the project 
a window with two blanck grids pop up:


IMAGE GRILLE VIDE

The left click lets the user place the start (the orange square), the end (cyan square) and the walls (black tiles) in this order of priority. 
If there is no start, it will place the start, if there is a start but no end, it will place the end and if both start and end are already placed, it will place a wall.
The user can remove a tile place simply by right clicking it. 
The user can also reset the grids just by pressing the C key.
The user can also randomize the map by pressing the "random map" button.


IMAGE GRILLE PLEINE

Once the user choosed how he wanted to placed every tiles, the user can start running the algorithm by pressing the SPACE key. 
The A star algorithm will start running and will try to find the shortest path, if the A star found one, the Djikstra algorithm start.
The shortest path will be highlighted by coloring yellow the tiles of the path between the start and the end.
A tile that was treated by an algorithm will be colored red and the next waves of tiles to be treated are colored green.


IMAGE GRILLE RUN

If the A star algorithm doesn't found any path and can't progress any further, the Djikstra algorithm will not start.

IMAGE GRILLE BLOQUE
 





