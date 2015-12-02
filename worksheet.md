# Weightlessness Mooncake in Space

In space, it feels like everything is floating. This is because everything becomes **weightless** outside of our planet, Earth. This is probably the biggest difference from being on Earth, where everything, and everybody, is pulled down towards the ground. On Earth, we can all feel this downward pull, but we are so used to it that we sometimes do not even think about it. This pull or attraction we feel is called **gravity**.

You can recreate the effects of weightlessness in Space in this Scratch game.

## Set the stage with a space theme

1. If you are using a Raspberry Pi you can open Scratch by clicking on **Menu** and **Programming**, followed by **Scratch**. Alternatively you can use Scratch 2.0 online for this activity altho some of the blocks may be slightly different. 
1. Create a new file by selecting **File** and **New**.
1. Delete the Scratch cat sprite by right clicking on it and selecting **Delete** from the menu that is displayed.
1. For this project, you need to create a new background to act as the Earth. To do this, click on `stage` in the sprites palette and then click on `Backgrounds` next to the `scripts` tab.
1. Click on `Paint` to draw your own background. Select the rectangle icon and a green colour. It is important that you fill the rectangle with one solid colour. Once you are happy with your stage design click **OK**. 	
1. You can use the Scratch cat sprite or alterntively you can use our [Mooncake - the Astro Cat sprite](files/Astro-cat.png). If your Raspberry Pi is connected to the internet you can download this sprite using the link. Save the image somewhere that you will be able to find it later on your Raspberry Pi.
1. Next add a new sprite by clicking on the `import a new sprite` icon on the sprites palette (which looks like the image below) and select `Astro-cat.png` from the choices and click **Ok**.

	![import new sprite](images/import-sprite-icon.png)
	
1. Click on the `costumes` tab for the Mooncake sprite. You will see one costume listed. Click on **import**. This time select [Mooncake - the Astro Cat sprite version 2](files/Astro-cat2.png). You will see two Mooncake costumes - one with a backpack firing and one without flames. You will use these costumes within your game to show that Mooncake moving. 
	  	
1. Click on the `scripts` tab of the sprite and save your Scratch project work by clicking on **File** and **Save As**. Name your progam **weightless** and save it in your home directory or some place that you can find it later.

## Setting the start position

1. Open the `Control` blocks area and begin by dragging a `When green flag clicked` block into the main script area.

1. To make sure that Mooncake starts at the top of the screen at the start of the program you will need to set the coordinates. Use a `go to x: 0  y: 0` block from the `Motion` blocks area. Drag it over and clip it beneath `When green flag clicked`.

1. Drag a `point in direction` motion block and connect it to your script.

1. Click on the **Control** blocks and add a `broadcast` block. Select **New** from the drop-down menu. Name the new broadcast message `start`.

	![](images/new-broadcast.png)

	A broadcast block with a unique message is used to coordinate the actions of different sprites and the stage in scratch.

## Adding movement

As Mooncake is in Space, she would be experiencing the effects of weightlessness and float about. We've given her a backpack so that she can change direction thanks to a force of energy. You see without a backpack or anything to push against, Mooncake would just keep going in one direction!

1. With the Astro-cat sprite selected, click on the control blocks and add a `when I receive` block to the stage. Select **start** from the drop down list. Remember this is the message that is broadcast by your first script.

1. Next add a `forever` looping block undrneath. 

1. Inside the forever loop add a `move 2 steps` block. 

1. Save your work so far and click on the green flag to test your scripts work as expected. Mooncake should move in one direction until she reaches the edge of the stage.

	![](images/move-code.png)

## Adding directonal movement

Let's control the direction of Mooncake the Astro Cat with code. 

1. Add another `when green flag clicked` control block to the scripts area for your sprite. 

1. connect a `forever` looping block.

1. Then add an `if else` control block inside the loop. 

	Conditional blocks like `if` and `if else` allow you to set a condition, that if met triggers something to happen. For example you will set the condition here that if the left arrow key has been pressed then point the sprite left and switch the sprite costume so that it looks like her jet pack is firing. Else, use the first costume.

1. To set a condition in scratch you need to add some blocks into the space next to the word if. Drag a `key space pressed` sensing block and put it into the space. Using the drop down menu select `left arrow`.

1. Inside the `if` part of the if else block put a `point in direction` movement block. Set the direction to left or `-90` degrees. 

1. Underneath add a `switch to costume` block and select your second sprite costume (the one with the flames coming out of the jet pack).
	
	![](images/direction-code.png)

1. Save and test that your direction arrow works. You will need to repeat this step for each direction that you want to move in, e.g. up, down and right. What values would you need to change for each direction?	

## Wrapping space

Mooncake the Astro Cat's movement is programmed to be automatic. This means that when she hits the edge of the stage she stops. You can add some code to make the sprite reappear on the other side when she goes off screen to give the appearance of endless space. This is called wrapping. 

1. Add a `When I recieve` control block onto the scripts area for your Mooncake sprite. Select **start** from the drop down list.

1. Next connect a `forever` loop to the control block. Inside the forever loop add a `Move 2 steps` motion block. 

1. Underneath the move block, connect an `if` control block. This block has a space to add other blocks to set the condition. 

1. Click on the operators blocks and select the greater than or equal to block which has this symbol `<`. Drag the block and place it insde the if space. 

1. On the left side of the `<` symbol add a `x position` movement block. Then on the right side type `240`. 

1. Inside the if block place a `set x to ` block and type the value `-240`. 

	This sets the condition that if the position of the sprite on the x axis is 240 then move the sprite to -240 on the same axis. So if the sprite goes off the right hand side of the screen then she will repear on the left. You will need to repeat the steps above for the left hand side of the screen but remember to switch the values so that the x position is greater than or equal to `-240` and the `set x to ` block value is `240`. 

1. Now you will need to add two more conditions for the top and bottom of the screen. Repeat the steps above but this time use the values for `y` axis `180` and `-180`. Check the image below against your code to check that your values are correct.

	![](images/wrapping.png)

## Make a game of it with variables
A way to keep score during the game is required. You can use a variable in your code to so this. A variable is a fancy name for storing data for use later on.

1. To create a variable, click on `Variables` in the blocks palette and then click `Make a Variable`. The `New Variable` window opens and asks you to type a name for your variable.
1. Name the first variable `score` and ensure that `For all sprites` is checked before clicking **OK**.
1. You’ll see some orange blocks are added to your Variable area called score, and a small counter box will appear on the stage.
1. Create another variable called `Time` that you can use to time each game. 

## Catch the randomly moving ISS

Mooncake needs something to chase in order for this program to become a game for people to play. This could be cat food, aliens or even a space mouse! We've used an image of the International Space Station for Mooncake to try and reach but you don't have to. Simply follow the steps and replace the sprite with whatever you would like to use. 

1. If your Raspberry Pi is connected to the internet you can download [this ISS sprite](files/iss.png) using the link. Save the image somewhere that you will be able to find it later on your computer or Raspberry Pi.
1. Next add a new sprite by clicking on the `import a new sprite` icon on the sprites palette and select `ISS.png` from the choices and click **OK**. Another sprite will be added to your sprites palette. 
1. Click on the ISS sprite to select it. A blank scripts area will appear. This is where you will write the code that affects this sprite. 
1. Begin by placing a `When I receive` control block to the scripts area. Using the drop down menu select `start`. 
1. Connect a `hide` looks block underneath, followed by a `wait 1 secs` block and then a `show` looks block. 
1. To make the game interesting, let's use some code the make the ISS randomly appear at different places across the screen. To do this add a `set x to ` block to the script. And inside the space add a `pick random` block and change the values to `-220 to 220`. This will place the ISS sprite on the x axis on the screen anywhere between -220 and 220. Repeat this step for the y axis to `set y to pick random -160 to 160`. 

	This code will allow the ISS sprite to appear randomnly once. Mooncake would easily be able to reach it and the game would be over. You can add some code so that each time Mooncake catches the ISS, it reappears randomly elsewhere. 

1. Underneath the last block add a `forever if` conditional loop. Inside the space on the block drop in a `touching ?` sensing block. Using the drop down arrow select the Astro cat sprite.   
1. Inside the forever if loop add a `change score by 1` variable block. Each time the player reaches the ISS sprite the score will go up by 1 point. 
1. Then repeat the code you used to randomly place the ISS on the screen like this:

	![](images/chase-iss.png)
1. Save your work by clicking on **File** and **Save**.
2. 
## Creating a Game Over screen

First you need to add a new Game Over background to the stage. You could paint or import a new one, but here we will duplicate the existing space background and edit it to display Game Over across it in large letters. 

1. Click on the **stage** icon and then click on **backgrounds**. Make a copy of the space background by clicking on **copy**. 

1. Now click on **Edit** to open the paint editor window. Using the text tool type 'Game Over' in large letters on the background. You can choose a colour and font that you like. When you are happy with how it looks click on **OK**.

	![](images/edit-background.png)

1. Next click on the **Scripts** tab and add a `when green flag clicked` control block to the scripts area. Note that the scripts area on the stage should be empty. All your other scripts are on your sprites.

1. Add a `switch to background` look block underneath. Select **space background** from the drop down box. This is the stage that you want the game to start with. 

1. Now add a `forever if` block to the script. Place an equals operator block inside the hexagon section of the forever if block. Click on the variables blocks and drag the `time` variable block and add it to the left hand side of `=`. Type `30` into the right hand side `=`.

1. Then inside the foerver if block, place a `switch to background` block. Select **space background1** from the drop down list. This should be your game over screen. 

1. Finally add a `stop all` control block underneath the last block. The Stop All control block will stop all the scripts in Scratch from running, ending the game.

	![](images/game-over-script.png)
1. Add the control block broadcast and create a new broadcast message called Game Over.
1. Save your game and test that it works by clicking on the green start flag. 

	![](images/finished.png)	
	
## What's next?	
- You could make the game more interesting by adding extra sprites for Mooncake to reach. PErhaps some of them could give her a speed up or a slow down. Adding osticles could also be a fun way to add more excitment to your game. 
- If you have a [Sense HAT](https://www.raspberrypi.org/products/sense-hat/), could you use it to trigger the timer instead of pressing the space bar?
- Check out some of our other [Space themed projects](https://astro-pi.org/resources/). 