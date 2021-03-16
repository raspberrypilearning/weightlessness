## Control direction

Astronauts can control the direction of their movements. The character in your game will be controlled using the keyboard arrow keys.

First, add a new script to move your character sprite upward when you press the up arrow key.

--- task ---

Drag a `when space key pressed`{:class="block3events"} block to an unused space in your Code area. Add a `point in direction`{:class="block3motion"} block underneath it:

![the Ripley sprite icon](images/ripley-sprite-icon.png)

```blocks3
when [up arrow v] key pressed // update key to up arrow
point in direction (0) //direction 0 is pointing up
```

**Test:** Click on the `green flag`{:class="block3events"} to run your project. Press the up arrow to see your character sprite move upward. 

--- /task ---

You'll need to add three more scripts to move left, right and down. When you set up your character you added a `point in direction 90`{:class="block3motion"} block to point to the right. Can you work out what values you need to point left and down?

--- task ---

Create three more scripts using `when space key pressed`{:class="block3events"} and `point in direction`{:class="block3motion"} blocks:

![the Ripley sprite icon](images/ripley-sprite-icon.png)

```blocks3
when [right arrow v] key pressed // update key to right arrow
point in direction (90) //direction 90 is pointing to the right
```

```blocks3
when [left arrow v] key pressed // update key to left arrow
point in direction (-90) //direction -90 is pointing to the left
```

```blocks3
when [down arrow v] key pressed // update key to down arrow
point in direction (180) //direction 180 is pointing down
```

**Test:** Click on the `green flag`{:class="block3events"} to run your project. You can now move your character sprite in all directions.

--- /task ---

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**Arrow keys**</span> are often used to control directional movements of a character in video games. Can you think of any other games that use arrow keys to control the player's character? 
</p>

--- save ---