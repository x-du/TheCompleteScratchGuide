# 15-Puzzle

The 15-puzzle \(also called Gem Puzzle, Boss Puzzle, Game of Fifteen, Mystic Square and many others\) is a sliding puzzle that consists of a frame of numbered square tiles in random order with one tile missing.

{% embed url="https://en.wikipedia.org/wiki/15\_puzzle" %}

## Finished Game

{% embed url="https://scratch.mit.edu/projects/380020934/" %}

If you want to know how to solve this puzzle, you can check this instruction: 

{% embed url="https://www.instructables.com/id/How-To-Solve-The-15-Puzzle/" %}

## Game Design

When we design the game we need to think about the following questions?

![](../../../.gitbook/assets/screenshot-2020-03-28-00.54.12.png)

## Game Board Design

Draw a backdrop that looks like the one in the image. 

![](../../../.gitbook/assets/screenshot-2020-03-28-00.56.56.png)

If you don't know how to draw rounded corner, check this [youtube video](https://www.youtube.com/watch?v=vywd08v8KD0). 

## The size of the tile

We are going to use the method illustrated in the image to calculate the tile size. 

![](../../../.gitbook/assets/screenshot-2020-03-27-23.17.18.png)

Use this trick to figure out the Max\_Y, Max\_Y, Min\_X and Min\_Y. 

![](../../../.gitbook/assets/screenshot-2020-03-28-01.06.18.png)

## Create tiles 1 to 15, and a blank tile

![](../../../.gitbook/assets/screenshot-2020-03-28-01.09.57.png)

![](../../../.gitbook/assets/screenshot-2020-03-28-01.14.50.png)

## Data Structure - List 

We are going to create list with number 1 to 15 at the random position, and have the value 16 at position 16. 

Not all random combinations are solvable. Actually half of them are not solvable.  The function cal\_inversion is used to check if the game is solvable. If the Inversion is an even number it is solvable. 

You can learn more about the algorithm here:

{% embed url="https://www.cs.bham.ac.uk/~mdr/teaching/modules04/java2/TilesSolvability.html" %}



![](../../../.gitbook/assets/screenshot-2020-03-28-01.25.21.png)

#### The relationship of \(row, column\) and index. 

![](../../../.gitbook/assets/screenshot-2020-03-28-01.37.54.png)

## Local variables for Tile

* r:  row 
* c: column
* value: the number in the tile.  The value is also the index of the costume. 

## Moving the tile

![](../../../.gitbook/assets/screenshot-2020-03-28-01.56.40.png)

1. Find the empty title. 
2. Swap  the tile next to the empty tile, depends on the arrow key.
3. Check if the list is sorted. 

## Check if the puzzle is solvable

Half of the random generated puzzles are not solvable. You can check if the puzzle is solvable using inversion counting method. 

{% embed url="https://www.geeksforgeeks.org/check-instance-15-puzzle-solvable/" %}

![Check if the puzzle is solvable](../../../.gitbook/assets/screenshot-2020-04-11-23.55.48.png)

## Check Win

If the list is sorted from small number to large number, the puzzle is solved. 

![](../../../.gitbook/assets/screenshot-2020-04-12-00.02.15.png)

## Track the best score

![](../../../.gitbook/assets/screenshot-2020-04-12-00.00.06.png)

## 

