# unofficialhashpluspluscommands
Hi! Here you will find community commands that we personally added here for the command-line version of HashPlusPlus

Build a command kit


### How do I make a command?
Here's a one argument example:
```json
{
    "name": "Greeting",
    "triggercommand": "greet",
    "description": "Greets someone by name.",
    "usage": "greet <person>",
    "args": 1,
    "arguments": {
        "arg1": "person"
    },
    "script": "print(f'Hello, {person}!')"
}
```
What does this mean?
| Field | Description |
| --- | --- |
| `name` | A readable name for your command. |
| `triggercommand` | What the user types to run it. Choose a unique trigger command that does not match any built-in commands. |
| `description` | A short explanation shown in help. |
| `usage` | How to use the command, including any arguments. |
| `args` | The number of arguments the command requires. |
| `arguments` | Maps each argument number to a Python variable name. |
| `script` | Python code to run when the command is used. |

How do I make my own?

Easy, first think of a name and make a file of it, with the file extension as `.json`, where you can add basic formatting:
```json
{

}
```
Now think of the following things:
"What do I want it's `name` to be?"
then simply write:
```json
{
  "name": "your choice of name here",
}
```

"What do I want the users to type to `trigger the command`"
then add:
```json
"triggercommand": "your trigger command here",
```

"How should it be `described` to my users?"
add it.
```json
"description": "your description here",
```

"Wait, how are my users going to know how to `use` it?"
```json
"usage: yourcommand <anyarguments>",
```

"I want my users to actually be able to write `arguments` if there are any."
You'll want to think how much you want so you can add:
```json
"args: {num},"
```
followed by:
```json
"arguments": {
  "arg1": "howyouwanttowriteitinyourscript",
  "arg2": "example"
},
```

"Finally, now how do I make it ACTUALLY `work`."
Add:
```json
"script": ""
```
And as for the script.. you do anything! Just know:

Want to reference an `arg`? Make sure to use the `variable name` you referenced, such as for arg1 in the 'greet' example, you would use `person`.

Want to add a new line? Don't press enter, just put in:
```json
\n
```
may be hard, but perfect takes practice.

## We don't expect you to get it first try!
## Report Issues here.



