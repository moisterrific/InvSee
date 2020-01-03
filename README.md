InvSee
======
[TShock](https://github.com/NyxStudios/TShock/) plugin. Utilizes SSC technology to copy a player's inventory.


### Commands ###
`invsee (-s[ave])|<player name>` - The main command. Will copy target player's inventory, if possible. Will also generate a backup of your character's inventory. The backup will only be generated if one is not in place -  this prevents the loss of your precious items when copying multiple players in a row. If, while copying a player's inventory, you wish to make any changes to it, you may change it at will and then execute `invsee -s` to save any changes made to that player's inventory. Last but not least, use `invsee` with no parameters to restore your inventory, destroying the backup in the proccess (simple, huh?).

Inventories are automatically restored upon leaving. Crashes and connection losses are exceptions - try not to hang around with other's inventories for too long. A fix might be implemented in the future.


### Permissions ###
`invsee.main` - Required to use the `invsee` command.

`invsee.save` - Required to save changes made to a player's inventory.

`invsee.user` - Combine with the above to allow copying offline players (users).

*Requires ServerSideCharacters
​
Since the similar feature currently present in Essentials by Scavenger seems broken, and Essentials+ did not adopt this (I don't see how could this be "Essential" for a server), I decided to use my spare time in reworking this from the core. TShock now includes its own methods for managing this copypasta, which makes it fairly easy to put this to work.

You can use this with Essentials: it should replace the old command with this one.

Features: 
An easy, and interactive way of reading player inventories by having your own replaced by theirs temporarily!
Creates a backup of your own inventory, and restores it automatically on leave or through the use of a command. I wouldn't want you to lose your inventory in the proccess of looking for hackers.
It is now safe to copy multiple inventories in succession: the backup will always contain your original inventory.

invsee.main - Required to use the invsee command.

invsee.user - Combine with the above to allow copying offline players (users). 

https://tshock.co/xf/index.php?resources/invsee.50/
