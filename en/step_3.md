## Add weightlessness

Your character is in space and will be floating around experiencing the effects of weightlessness. 

At the moment, your character sprite is quite big so your game will be too easy!

--- task ---

From the Sprite pane, click on the **Size** property and change the value to `50`%:

![Sprite pane with size set to 50 percent.](images/size-property.png)

--- /task ---

A group of connected blocks in Scratch is called a script. You will add a script to your character sprite so it starts in the middle of the Stage then moves `forever`{:class="block3control"} through space. 

--- task ---

Click on the `events`{:class="block3events"} blocks menu and drag a `when flag clicked`{:class="block3events"} block to the Code area. Connect some `motion`{:class="block3motion"} blocks to the bottom of your script to get your character sprite ready to move:

![The Ripley sprite icon.](images/ripley-sprite-icon.png)

```blocks3
when green flag clicked
set rotation style [left-right v]
go to x: (0) y: (0)  //The middle of the screen
point in direction (90) //Facing the right
```

![The scratch editor showing the script in the Code area.](images/first-code.png)

--- /task ---

--- task ---

**Test:** It is a good idea to test your project regularly in full screen mode using the **Full Screen Control**. This view will let you see your game the way a user playing your game would see it.

To run your project in full-screen mode in Scratch, go to the area above the Stage and click on the icon with four arrows that point outwards. This is the Full Screen Control icon:

![The icons on the top of the Stage with the far left icon 'full screen mode' highlighted.](images/full-screen-mode.png)

Click on the `green flag`{:class="block3events"}, your character sprite will move to the middle of the Stage.

To exit full-screen mode, click on the Full Screen Control icon again. It will have four arrows that point inwards.

--- /task ---

--- task ---

Add a `forever`{:class="block3control"} loop to the bottom of your script. Insert `motion`{:class="block3motion"} blocks inside your `forever`{:class="block3control"} loop to create weightless movement:

![The Ripley sprite icon.](images/ripley-sprite-icon.png)

```blocks3
when green flag clicked
set rotation style [left-right v]
go to x: (0) y: (0)  //The middle fo the screen
point in direction (90) //Facing the right
+ forever
move (2) steps
if on edge, bounce //Turn around at edge of the Stage
```

**Test:** Enter full screen mode then click on the `green flag`{:class="block3events"}, your character sprite will float across the Stage.

--- /task ---

--- save ---
