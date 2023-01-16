# Introduction

Variables are like holders for values, and these values can be different types. These are used to make the code easier to write and read, as it can shorten
a long value to a short word. You should know the types of variables if you want to be a good programmer, and try to not memorize them but understand them.

# Creating a Variable

You will need a name for the variable, and a value.

```lua
myVariable = "this is a cool variable"
print(myVariable)
```
myVariable here represents the string `this is a cool variable`, and it will be printed using the print function. (Functions will be explained later on)

# Variable Types

- `string`  | This is used for text, like a character, a word, a sentence, or anything that is contained between two quotes.
- `number`  | This is used for numbers.
- `boolean` | This is used for `true` and `false` values. (Which means yes and no, but the programming way)
- `nil`    | This represents nothing. Nil means the variable isn't assigned to any value.

# Examples

```lua
stringVariable = "This is a string."
numVariable = 12345
boolVariable = true -- This can also be false.
emptyVariable = nil
```

# Local Variables

Variables can be global or local. Global variables can be used anywhere in the script, and to make a variable local, you will need to add the word `local`
before adding a value. For example:

```lua
myNumber = 1

if myNumber == 1 then -- You will learn about if statements later on.
  globalNum = 5
  local myString = "This is my string"
  print(myString) -- This will print myString without any problems.
end

print(myString) -- This won't work because myString is only available inside of the if statement.
print(globalNum) -- This will work even though globalNum is defined inside of the if statement, and that's because it's not local.
```
