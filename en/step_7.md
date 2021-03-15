## Create a Game Over screen

Game over screens are a great way to end video gomes. Some have a simple 'game over' message whilst others have details of who made the game and may even feature all the sprites involved in a game. 

To create a game over screen you'll need to add a backdrop and edit it with colours, shapes or text.

--- task ---

Click on the **Choose a backdrop** button. If you want to continue your space theme, click on the **Space** category. We chose **Nebula** but you can choose any backdrop you like:

![Choose a backdrop button](images/choose-backdrop-icon.png)

--- /task ---

--- task ---

Click on the **Backdrops** tab and you will see the backdrops currently in your project with your new backdrop at the bottom of the list. 

![Backdrops tab with new backdrop highlighted](images/nebula-editor.png)

--- /task ---

Edit your backdrop to include some text. 

--- task ---

Click on the **Text** tool:

![The text tool icon](images/text-icon.png)

Choose the colour and font style you want from the drop down boxes: 

![The fill chooser tool and font style drop down](images/text-properties.png)

**Tip:** Use the sliders in the **Fill** colour chooser to pick your colour. If the colours turn only to black or white you might need to adjust the **Saturation** or **Brightness** sliders.

--- /task ---

--- task ---

Click where you want the text to appear on the backdrop then type 'Game Over' or words of your choice.

![Game Over wording on the Nebula backdrop in the editor](images/nebula-with-text.png)

--- /task ---

Set up you game to start on your first backdrop then change to the Game Over backdrop at the end.

--- task ---

Click on you character sprite, at the end of your `set score to 0`{:class="block3variables"} script, add a `switch backdrop`{:class="block3looks"} block:

![the Ripley sprite icon](images/ripley-sprite-icon.png)

```blocks3
when flag clicked 
set [score v] to (0)
+ switch backdrop to [Galaxy v] // switch to your main backdrop
```

--- /task ---

--- task ---

Find your `when timer > 30`{:class="block3events"} script and insert a `switch backdrop`{:class="block3looks"} block at the top.

![the Ripley sprite icon](images/ripley-sprite-icon.png)

```blocks3
when [timer v] > (30) // 30 second after flag clicked
+ switch backdrop to [Nebula v] // switch to your Game Over backdrop
say (score)
stop [other scripts in sprite v] 
```

**Test:** Run your project. Does your backdrop change to the Game Over screen? When you run it for a second time does it switch back at the start of the game?

--- /task ---

--- save ---
