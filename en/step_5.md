## Setting the start position

- Open the `Control` blocks area and begin by dragging a `When green flag clicked` block into the main script area.

- To make sure that Mooncake starts at the top of the screen at the start of the program, you'll need to set the coordinates. Use a `go to x: 0  y: 0` block from the `Motion` blocks area. Drag it over and clip it beneath `When green flag clicked`.

- Drag a `point in direction` motion block and connect it to your script.

- Click on the **Control** blocks and add a `broadcast` block. Select **New** from the drop-down menu. Name the new broadcast message `start`.

	![](images/new-broadcast.png)

	A broadcast block with a unique message is used to coordinate the actions of different sprites and the stage in Scratch.

