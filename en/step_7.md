## Adding directonal movement

Let's control the direction of Mooncake the Astro Cat with code.

- Add another `when green flag clicked` control block to the scripts area for your sprite.

- Connect a `forever` looping block.

- Then add an `if else` control block inside the loop.

	Conditional blocks like `if` and `if else` allow you to set a condition that, if met, triggers an event. For example, you'll set the condition here that if the left arrow key has been pressed, then the code will point the sprite left and switch the sprite costume so that it looks like her jetpack is firing. If the key is not pressed, it will use the first costume.

- To set a condition in Scratch, you need to add some blocks into the space next to the word `if`. Drag a `key space pressed` sensing block and put it into the space. Using the drop-down menu, select `left arrow`.

- Put a `point in direction` movement block inside the `if` part of the `if else` block. Set the direction to left or `-90` degrees.

- Underneath, add a `switch to costume` block and select your second sprite costume (the one with the flames coming out of the jetpack).

	![](images/direction-code.png)

- Save and test that your direction arrow works. You'll need to repeat this step (duplicating the code block above) for each direction that you want to move in, i.e. up, down, and right. What values would you need to change for each direction?

