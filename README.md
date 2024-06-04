# GodotDragAndDrop
Repo to store the code I wrote following a tutorial for a drag and drop system in Godot.

I followed [this tutorial](https://youtu.be/uhgswVkYp0o?si=s26DOPmsDC1q2hOT)

## Missing steps

Note: this is not meant to critisice the tutorial as godot is a changing product and the tutorial might hav been completely accurate at time of publishing

### Input Map "click"

Go to "Project" -> Project Settings" -> Input map -> in "add new action" write "click" (without the quotes) and press "Add"
Then press the + button next to the action name and add "Mouse Buttons" -> "Left Mouse button" to the list

### Area 2D sizes

While the platform ColorRect size change is mentioned, the size of the CollisionShape2D size is either not mentioned or mentioned superficially and I missed it.

### Color background not mentioned

This might be just my lack of experience with Godot but they don't mention anywhere where/how to change the background color on the scene

## Things I would change

I don't love that the draggable object is the one changing the color of the platform.
How the platform reacts to the object's prescence (or lack there of) should be up to the platform itself. 
If I had the time to tweak this example more I would emit a custom signal with either an ID or the position so that each platform can react wither the object entered them or not.  
The problem with this approach is that it would need an ID generation solution.
