### Command Pattern

Command pattern at its simplest decouples actions from their requests. This is done by creating a standalone intermediate object that gets sent by a sender/invoker, and passes along the request to a receiver.

Senders are loaded with command objects

Command objects are invoked with an execute method that calls the appropriate method on the receiver

Receiver objects need no change besides maybe having a reference to a command. They do the actual job that's done and that's it.

### Project 4

This project may appear overwhelming but don't worry, it's not all that bad. 

#### Parsing

The grammar for the command language is small. 

```
<command> <database id> <key> [<value>] | B | E
```

This means there are 3 potential inputs.

Either a B indicating a beginning for a macro, an E indiciating an ending for a macro, or a command line.

It's the Command, which database, a key, and then an optional value for the key. 

Your CS projects generally involve reading some kind of string. There are a number of approaches you can do but a nice easy one is to do the following:

- Readline, and then check the first element of the string you read. Check if B or E, otherwise it's a command, and then you can access the string by elements to set up the commands.

#### Structuring

You should have modules that are structured in a commandish form, you'll have a module for commands, one for your receiver, one for your invoker. 

Databases are receivers, your commands are commands, and you'll write a class that can handle sending requests. The Sender class will have a container for storing the commands, and ideally, it should also have a container for storing them for undo functionality.

#### Queuing



#### Undo
