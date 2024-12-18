<h1>Module-X</h1>

 <small>[By Roller_Bott](https://www.roblox.com/users/1219475555/profile)</small> | <small>Github</small> | <small>Download</small>

<p>This module was created to give scripters additional functions that ultimately make their jobs easier. These functions can be created and run without this module, but having the module cleans up code and makes it more readable while also making scripting more enjoyable.</p>
<br>
<hr>
<h1>Setting Up the Module</h1>


This line of code is necessary before you can call anything from the module. 
Obviously, this can be optimized, though it is not used often.

```lua
local ModuleX = require(script.Parent:WaitForChild("Module-X"))
 ```
After requiring the module, you will want to choose an instance and assign a variable to `version.createGhost()` and put your **[Instance](https://create.roblox.com/docs/reference/engine/datatypes/Instance)** in between the two parentheses. The new variable is called the **ghost** *(As in the ghost of the original part)*. *See Figure 1 below*
```lua
-- Figure 1
local ModuleX = require(script.Parent:WaitForChild("Module-X"))

local part = Instance.new("Part")
local partGhost = ModuleX.createGhost(part)
```
Understand that a ghost provides extra features for the instance it is linked to. It is not an instance in itself, so you cannot parent things to the ghost.

> **Ghosts** <br>
Think about the properties tab. Each value is in a section. Think of ghosts as another section. This section comes with useful functions and one value (`Cognate`) that tells the ghost which instance it is binded to. Whatever available function used on a ghost is actually being used on the part!

<br>
<br>
<hr>
<h1>Documentation</h1>

