## Catch the randomly moving ISS

Mooncake needs something to chase in order for this program to become a game for people to play. This could be cat food, aliens or even a space mouse! We've used an image of the International Space Station for Mooncake to try and reach but you can use what you like. Simply follow the steps and replace the sprite with whatever you would like to use.

- If your Raspberry Pi is connected to the internet you can download [this ISS sprite](resources/ISS.sprite) using the link. Save the image somewhere that you'll be able to find it later on your computer or Raspberry Pi.

- Next, add a new sprite by clicking on the `import a new sprite` icon on the sprites palette, then select `ISS` from the choices and click **OK**. Another sprite will be added to your sprites palette.

- Click on the ISS sprite to select it. A blank scripts area will appear. This is where you'll write the code that affects this sprite.

- Begin by placing a `When I receive` control block into the scripts area. Using the drop-down menu, select `start`.

- Connect a `hide` looks block underneath, followed by a `wait 1 secs` block and then a `show` looks block.

- To make the game more interesting, let's use some code that makes the ISS randomly appear at different places across the screen. To do this, add a `set x to ` block to the script, then inside the space add a `pick random` block and change the values to `-220 to 220`. This will place the ISS sprite on the x axis on the screen anywhere between -220 and 220. Repeat this step for the y axis to `set y to pick random -160 to 160`.

	This code will allow the ISS sprite to appear randomly once. Mooncake would easily be able to reach it and the game would be over. You can add some code so that each time Mooncake catches the ISS, it reappears randomly elsewhere.

- Underneath the last block, add a `forever if` conditional loop. Inside the space on the block drop in a `touching ?` sensing block. Using the drop-down arrow, select the Astro Cat sprite.   

- Add a `change score by 1` variable block inside the `forever if` loop. Each time the player reaches the ISS sprite, the score will go up by 1 point.

- Then repeat the code you used to randomly place the ISS on the screen like this:

	![](images/chase-iss.png)

- Save your work by clicking on **File** and **Save**.


