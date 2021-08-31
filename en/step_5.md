## Catch a sprite

Your character needs an object to chase. Your object could be an item or another character. What will you choose? We used the **Dot** space dog sprite, but you can use whatever you like. 

--- task ---

Click on the **Choose a Sprite** button to see the available sprites. Find one you like, and click on it to add it to your project:

!['Choose a Sprite' button.](images/sprite-button.png)

**Tip:** You'll need to change the size again so it suits your game:

![Stage with two characters correctly sized.](images/stage-two-characters.png)

--- /task ---

Add code to make your object sprite appear in different places each time the `green flag`{:class="block3events"} is clicked.

--- task ---

Drag a `when flag clicked`{:class="block3events"} block to your object sprite. Use `hide`{:class="block3looks"}, `go to random position`{:class="block3motion"}, `wait`{:class="block3control"}, and `show`{:class="block3looks"} blocks so your object sprite appears in a surprise position:

![The Dot sprite icon.](images/dot-sprite-icon.png)

```blocks3
when flag clicked
hide //Disappears from the stage
wait (1) seconds //Builds suspense
go to [random position v] //Moves to new position
show //Appears on the Stage
```

**Test:** Run your project a couple of times. Does your object sprite move to a different position each time?

--- /task ---

To turn your project into a game, the script needs to repeat every time your character sprite and object sprite touch.

--- task ---

Add a `forever`{:class="block3control"} loop to the bottom of your object sprite script and insert an `if`{:class="block3control"} condition block inside. 

To sense `if`{:class="block3control"} your sprites are touching, add a `touching mouse-pointer ?`{:class="block3sensing"} block and select your character sprite name from the drop-down menu:

![The Dot sprite icon.](images/dot-sprite-icon.png)

```blocks3
when flag clicked
hide //Disappears from the stage
wait (1) seconds //Builds suspense
go to [random position v] //Moves to new position
show //Appears on the Stage
+forever
if <touching [Ripley v]> then //Update block to show your character sprite
```

--- /task ---

--- task ---

Inside the `if`{:class="block3control"} block, add the same four blocks you used earlier:

![The Dot sprite icon.](images/dot-sprite-icon.png)

```blocks3
when flag clicked
hide //Disappears from the stage
wait (1) seconds //Builds suspense
go to [random position v] //Moves to new position
show //Appears on the Stage
forever
if <touching [Ripley v]> then
+ hide
+ wait (1) seconds 
+ go to [random position v] 
+ show 
```

**Test:** Run your project. Use the arrow keys to move your character. When your sprites touch, your object sprite will hide and re-appear in a new position. 

--- /task ---

--- save ---
