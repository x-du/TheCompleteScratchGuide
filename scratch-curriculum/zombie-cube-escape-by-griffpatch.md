# Zombie Cube Escape by Griffpatch

## What is this?

This is the [game](https://scratch.mit.edu/projects/284516654/) and [video tutorial](https://www.youtube.com/watch?v=GXsjYupfDYk&t=159s) created by [griffpatch](https://scratch.mit.edu/users/griffpatch/).  

{% embed url="https://scratch.mit.edu/projects/284516654/" caption="The Zombie Cube Escape Game on Scratch" %}

## Part 1 

In Part 1,  we will create a player and a ground for the game.  

* The player is a sprite that you can control with keyboard. 
* The ground \(Level sprite\) is the game's playground. One ground is one level. 

{% embed url="https://www.youtube.com/watch?v=GXsjYupfDYk&t=159s" caption="The Part 1 of the video tutorial on youtube. " %}

You can see my completed part 1 project at: 

{% embed url="https://scratch.mit.edu/projects/298618172/" caption="Completed Part 1" %}

### How to create a ground that is bigger than the scratch screen?

Create two costumes, one is small, the other is the real ground.  Switch to the small costume first, then change the size, then switch to the ground. 

![](../.gitbook/assets/screenshot-2019-04-13-21.14.04.png)

### Variables

* For Player only:  x and  y.
* For Level only: x and y.
* For all sprite: SCROLL\_X, and SCROLL\_Y.



### How to scroll the ground to the opposite direction, while keeping the player at the center of the screen?

In the run-loop:

1. Detect the key event to move the player.  \(See **Player Move** block and **Try Move** block.\).
2. Prepare the **Level** sprite to move to the opposite direction by changing **SCROLL\_X** and **SCROLL\_Y**.
3. Tell the **Level** and **Player** to move by sending the **Move Level** message. 

![The Player](../.gitbook/assets/screenshot-2019-04-13-21.20.24.png)

![The Level](../.gitbook/assets/screenshot-2019-04-13-21.45.34.png)



## Part 2

In Part 2,  we will create a zombie that follows the player. 

### Add a message to move zombie

![](../.gitbook/assets/screenshot-2019-04-13-21.26.52.png)

### The code for zombie

![Zombie](../.gitbook/assets/screenshot-2019-04-13-21.31.01.png)



## Part 3

Create multiple zombies and use a list to keep track of the zombie's position. 

New Variable: 

* MOBS:  a list to hold the positions of the zombies.

### How to create zombies 

![](../.gitbook/assets/screenshot-2019-04-13-22.25.11.png)

## Part 4

Add game over animation. 

![](../.gitbook/assets/end_game.gif)



![Player](../.gitbook/assets/screenshot-2019-04-13-23.12.05.png)

## Part 5



