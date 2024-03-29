# Introduction

Module scripts in Roblox are a way to organize and reuse code across multiple scripts. They are similar to functions in traditional programming languages, but they have additional features that make them useful for organization and sharing code. Module scripts are defined in a separate script file and can be imported and used in other scripts. [1](https://create.roblox.com/docs/education/coding-6/intro-to-module-scripts)

# Creating a Module Script

To create a module script, you will need to choose where you want to put it (preferably in `ReplicatedStorage`, because you might want some code to run for
clients), then just add a module script the same way you add a normal script.

# Exporting Values

To make values available for use in other scripts, you can use the `return` statement to export them from the module script. For example, the following module script exports a variable called `myValue` and a function called `myFunction`:

```lua
local myModule = {}

local myModule.myValue = 5

local function myModule.myFunction()
  print("Hello from MyModule!")
end

return myModule
```

# Importing a Module Script

To use a module script in another script, you can use the `require` function to import it. The following is an example of importing the `MyModule` module script and using the exported values:

```lua
local MyModule = require(game.ServerScriptService.MyModule)

print(MyModule.myValue) -- prints 5
MyModule.myFunction() -- prints "Hello from MyModule!"
```
