Introduction
------------

Vectors in Roblox Lua scripting are used to represent points and directions in 3D space. The two main types of vectors used in Roblox are Vector3 and Vector2. Vector3 represents a point or direction in 3D space with x, y, and z coordinates, while Vector2 represents a point or direction in 2D space with x and y coordinates.

Vector3
-------

Vector3 is used to represent a point or direction in 3D space with x, y, and z coordinates. The following is an example of creating a Vector3:

    local myVector3 = Vector3.new(1, 2, 3) -- creates a Vector3 with x = 1, y = 2, z = 3


Vector3 also has various methods to perform mathematical operations on vectors like adding, subtracting, multiplying, normalizing, etc. Here's an example of adding two vectors:

    local vector1 = Vector3.new(1, 2, 3)
    local vector2 = Vector3.new(4, 5, 6)
    local vector3 = vector1 + vector2 --vector3 = Vector3.new(5,7,9)


Vector2
-------

Vector2 is used to represent a point or direction in 2D space with x and y coordinates. The following is an example of creating a Vector2:

    local myVector2 = Vector2.new(1, 2) -- creates a Vector2 with x = 1, y = 2


Vector2 also has various methods to perform mathematical operations on vectors like adding, subtracting, multiplying, normalizing, etc. Here's an example of multiplying a vector with a scalar:

    local vector1 = Vector2.new(1, 2)
    local vector2 = vector1 * 2 --vector2 = Vector2.new(2,4)


Physics
-------

Vectors are commonly used in Roblox physics engine to represent position, velocity, and acceleration of an object in the game. Here's an example of applying force to an object:

    local myPart = game.Workspace.myPart
    local force = Vector3.new(0, 100, 0) -- creates a Vector3 with x = 0, y = 100, z = 0
    myPart:ApplyForce(force) 
These are some basic usage of Vector3 and Vector2, it is powerful tool in physics engine and you can do much more with it like raycasting, collision detection and so on. You can find more information and advanced usage in the Roblox developer documentation
