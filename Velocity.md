<h2>Introduction</h2>
<p>Velocity in Roblox Lua scripting is a vector that represents the speed and direction of an object's motion. Velocity is commonly used in Roblox physics engine to move an object in a certain direction. In Roblox, velocity is represented as a Vector3, which includes the x, y, and z components of the object's motion.</p>
<h2>Setting Velocity</h2>
<p>To set the velocity of an object, you can use the <code>Velocity</code> property of the object. The following is an example of setting the velocity of a part to move in the positive x direction:</p>
<pre>
<code>local myPart = game.Workspace.myPart
local velocity = Vector3.new(10, 0, 0) -- creates a Vector3 with x = 10, y = 0, z = 0
myPart.Velocity = velocity
</code>
</pre>
<h2>Getting Velocity</h2>
<p>To access the velocity of an object, you can use the <code>Velocity</code> property of the object. The following is an example of getting the velocity of a part:</p>
<pre>
<code>local myPart = game.Workspace.myPart
local velocity = myPart.Velocity
print(velocity) -- prints the velocity of the part as a Vector3
</code>
</pre>
<h2>Applying Force</h2>
<p>To apply a force to an object, you can use the <code>ApplyForce</code> method of the object. This method takes a Vector3 as an argument, representing the force to be applied in the x, y, and z directions. The following is an example of applying a force to a part to move in the positive x direction:</p>
<pre>
<code>local myPart = game.Workspace.myPart
local force = Vector3.new(100, 0, 0) -- creates a Vector3 with x = 100, y = 0, z = 0
myPart:ApplyForce(force)
</code>
</pre>
<h2>Friction</h2>
<p>Friction is a force that opposes motion of an object, you can use the <code>Friction</code> property of the object to set the friction. The value of Friction is between 0 and 1. The following is an example of setting the friction of a part to 0.1:</p>
<pre>
<code>local myPart = game.Workspace.myPart
myPart.Friction = 0.1
</code>
</pre>
<p>These are some basic usage of velocity and forces, you can find more information and advanced usage in the Roblox developer documentation</p>


