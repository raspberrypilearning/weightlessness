## Wrapping space

Mooncake the Astro Cat's movement is programmed to be automatic. This means that when she hits the edge of the stage she stops. You can add some code to make the sprite reappear on the other side when she goes off screen, to give the appearance of endless space. This is called wrapping.

- Find the `When I receive` control block you added earlier, it should look like this.

	![](images/move-code.png)

- Underneath the `move` block, connect an `if` control block. This block has a space to add other blocks to set the condition.

- Click on the operators blocks and select the greater than block which has this symbol `>`. Drag the block and place it inside the `if` space.

- Add an `x position` movement block on the left side of the `>` symbol, then on the right side type `240`.

- Place a `set x to ` block inside the `if` block and type the value `-240`.

	This sets the condition that if the position of the sprite on the x axis is 240, then the code moves the sprite to -240 on the same axis. So if the sprite goes off the right-hand side of the screen, then she will reappear on the left. You'll need to repeat the steps above for the left-hand side of the screen, but remember to switch the values so that the x position is greater than or equal to `-240`, and the `set x to ` block value is `240`.

- Now you'll need to add two more conditions for the top and bottom of the screen. Repeat the steps above, but this time use the values `180` and `-180` for the `y` axis. Check the image below against your code to check that your values are correct.

	![](images/wrapping.png)

