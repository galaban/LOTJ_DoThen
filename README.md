# Galaban's LOTJ Do/Then plugin
This is a rather large plugin that implements a #do and #then commands for the LOTJ Mud.

### Specifics

Let's say you get tired of typing "search" repeatedly.  This plugin adds allows you to type "#do search" and you will dig until you find something.  It's easy to image that after that you want to "get" whatever is on the ground.  With this plugin, you can enter "#then get camera".

Imagine that you want to develop 3 times.  Instead of using "#do develop", you can use "#do 3 develop" and it will stop after the third development.  (After that, I suggest "#then afk")

Other uses for #do or #then are:
* going AFK after development
* Repeating a development while botting
* Auto-repeating skills to train them, such as: study, research, slice, diagnose, locateship, lookup, and many more.

This is a very generic plugin.  

### Additional commands
There are a handful of other auto-repeat commands, such as

     #makearmor <armor>   - This repeats the "makearmor <armor>" command
     #dig
     #search
     #research *
     #study *

Also, there is a #autoslice command that will change the "secure ship" to "slice ship" one it is secured (and vice versa)

### Limitations
While I have made this as complete as I can, I have not played all the classes to completion.  In here, there are triggers for scientists, spies, and slicers.  Due to LOTJ's skill system, many other skills are covered.  However, for example, bounty hunters is completely untouched.

### Command Delay

This plugin incorporates an automatic delay into each repeat command.  So, for example, if you are digging, you won't immediately dig after the previous failed dig.

This delay is based on the command.  Digging and searching, for example, are shorter commands than development.

However, the delay is also random from N to N*2 seconds.  So, if the configured delay is 2 seconds, the actual delay will range from 2-4 seconds.  This just adds some variability to the commands.

### Legal Botting
There are also triggers in here that will watch to see if you are legally botting.  If so, the delay will be removed and the commands executed immediately.  Of course, make sure that you only "#do" commands that are legal to bot.  The imms are watching!

### Illegal Botting
DO NOT USE THIS PLUGIN TO BOT.

Yes, I realize that "#do diagnose" will continue until an imm disconnects you.  Also, I know that "#autoslice" seems to be a very direct bot.  In fact, every bit of this plugin seems to be botting.

Just, don't do it.

(OK... cya time is over.)
