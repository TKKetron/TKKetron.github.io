---
title: "Maze Generator"
excerpt: "A program for creating mazes using a multitude of algorithms with the ability to solve it <br/><img src='/images/Maze Generation/Mave Generator.png'>"
collection: portfolio
---

# Generator

This is one of my favorite personal projects. It taught me a lot about algorithms and taking a pre known set of instructions and converting it to code. My initial goal was to make a maze via code. This brought me to the wikipedia page containing many different algorithms for making one. I decided to challenge myself and use all of these algorithms.

Here you can see in my code the ability to generate different types of mazes based on the set of instructions provided in the original wikipedia article (might be slightly different)

![Different types](/images/Maze%20Generation/types.png)

for example, the provided algorithm in the above image was wilson's algorithm. This is the set of instructions i followed to generate a maze.    
    *Create a list of all walls, and create a set for each cell, each containing just that one cell.
    *For each wall, in some random order:
        *If the cells divided by this wall belong to distinct sets:
            *Remove the current wall.
            *Join the sets of the formerly divided cells.

Another thing this allowed me to do was test and improve my ability to work with inheritance. This was the perfect example of using a base class and object with a generate function in which I would override in each sub class. This allows for the main code that actually interacts with the visuals to be very simple and universal no matter how many different algorithms I added.

# Solver

With a maze able to be generated I needed to solve it. There were a few different solving algorithms I considered, but in the end A* is the most common and widely accepted as the standard option for most applications. I did this with the same challenge imposed from the start, that being just use a set of instructions to make the code with. This was a very difficult challenge and the result was VERY satisfying. Visualizing this in steps made the challenge also very difficult, but the result was worth it.

![Mid solve](/images/Maze%20Generation/mid%20solve.png)

Above you can see the maze being solved. Red shows tiles that have already been explored and checked. Green are next possible tiles to explore. Purple is destination, and finally Blue is in final path. At the start the only item in the final path is the starting tile because the path is not decided yet.

![Solved](/images/Maze%20Generation/Solution.png)

once the red is connected to the final destination it can begin to build the path by tracing back over the visited tiles getting the most efficient path. as you can see not every tile was visited before it had made a decision. This is the most efficient path and in this case there was only one solution, but even in an open path where multiple paths are possible it is guaranteed to find the shortest.

![Final Path](/images/Maze%20Generation/final%20path.png)

The final path is shown above. As you can see not even have of the mazed was explored yet it still has the path. Most mazes get to this result. The amount of maze explored depends largely on the algorithm used to generate the maze. For example A* does very poorly with the recursive maze generator that I made. This is due to the fact that it makes large pockets the A* algorithm is stuck exploring that we can see is a dead end.

![recursive solve](/images/Maze%20Generation/recursive%20solve.png)

# Other Functionality

This was a very large project and I still revisit it every now and then because it has many useful examples for me to reference. Similarly I use it as a testing program for new ideas. Recently I began making games, so for testing purposes I added a generate room and generate loot button to this program.

![Gen Rooms and Items](/images/Maze%20Generation/gen%20room%20and%20item.png)

Above shows the room and items generated, along with the solver working with those functionality. the solver goes straight through one of the rooms that was added. the items are that pink/red color and are just placed randomly.

This functionality allowed me to test teh A* solver implementation with open areas. this is more useful for pathing for AI in video games since usually spaces are open areas and not cramped hallways. Along with this the item generation Allows me to test item placement and density and is applicable in numerous other spaces.

Check all code for this project on my [GitHub](https://github.com/TKKetron/Maze-Generator)