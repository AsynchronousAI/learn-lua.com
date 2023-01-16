# Introduction

Loops in Roblox Lua scripting are used to repeat a block of code a certain number of times or until a certain condition is met. There are several different types of loops, including while loops, for loops, and nested loops, as well as the use of the `break` statement and the `wait` function.

# While Loops

A while loop is used to repeat a block of code while a certain condition is true. The following is an example of a while loop that counts from 1 to 10:

```lua
local count = 1
while count <= 10 do
  print(count)
  count = count + 1
end
```

# For Loops

A for loop is used to repeat a block of code a certain number of times. The following is an example of a for loop that counts from 1 to 10:

```lua
for count = 1, 10 do
  print(count)
end
```

# Nested Loops

A nested loop is a loop that is placed inside another loop. The following is an example of a nested loop that counts from 1 to 3 for each number from 1 to 2:

```lua
for i = 1, 2 do
  for j = 1, 3 do
    print(i, j)
  end
end
```

# Break Statement

The `break` keyword is used to exit a loop early. The following is an example of a while loop that counts from 1 to 10, but exits early when the count reaches 5:

```lua
for count = 1, 10 do
  print(count)  
  if count == 5 then break end -- Note: you can use if statements in one line like so.
  count = count + 1
end
```

# Wait

The `wait` function is used to make a script pause for a certain amount of time. It can be used inside a loop to create a delay between iterations. The following is an example of a for loop that counts from 1 to 3 with a 1-second delay between each count:

```lua
for count = 1, 3 do
  print(count)
  wait(1)
end
```

# Task.Wait()

The `task.wait()` function is similar to the `wait` function, but it is more accurate and recommended. It is mostly used when you want to
wait for a certain event to happen and do something else in the meantime.
