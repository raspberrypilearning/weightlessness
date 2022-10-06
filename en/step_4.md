## Control direction

Your astronaut is wearing a spacesuit with thrusters, allowing them to control the direction of their movements. 

--- task ---

Your program needs to continuously detect when the left mouse button is pressed. To do this, start a new script with a `when flag clicked`{:class="block3events"} block then add a `forever`{:class="block3control"} loop to your script. Inside the `forever`{:class="block3control"} loop add an `if ... then`{:class="block3control"} block to detect if `mouse down`{:class="block3sensing"}:

![The Ripley sprite icon.](images/ripley-sprite-icon.png)

```blocks3
when flag clicked
forever
if <mouse down?> then
```

--- /task ---

--- task ---

Scratch’s `mouse down`{:class="block3sensing"} block works for fingers on mouse buttons and on touchscreens!

To get the character sprite to respond to where the user clicks, add the following blocks: `if`{:class="block3control"} `mouse down`{:class="block3sensing"} `then`{:class="block3control"} the sprite should `point towards mouse-pointer`{:class="block3motion"} and `move 2 steps`{:class="block3motion"}:

![The Ripley sprite icon.](images/ripley-sprite-icon.png)

```blocks3
when flag clicked
forever
if <mouse down?> then
+ point towards (mouse-pointer) 
+ move (2) steps
end
```

--- /task ---

--- task ---

**Test:** Enter full screen mode then click on the green flag to run the program to test that your character faces and moves towards your mouse-pointer.

Make sure that your character moves in all directions.

--- /task ---

--- save ---
