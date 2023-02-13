
# Discord-Bot-Advanced
In the first workshop we learned how to create a basic bot. Now we will make it interract with other users and messages.

## Requirements
This workshop assume that you already have a [basic discord bot](https://github.com/FlorianLabarre/Basic-Discord-Bot#readme)
Since we will interract with server permission, we need to give them to our bot.

 1. Go to the [discord dev app](https://discord.com/developers/applications)
 2. Select your application
 3. In OAuth2 -> URL Generator select **bot** and **administrator**

## Exercice 1
Make a function that will **delete** a message if it contains a word in a **blacklist**

## Exercice 2
Make a slash command that can **delete multiple messages** in a channel
To create this command you will need to add **[options](https://discordjs.guide/slash-commands/advanced-creation.html)** like the number of message to delete

There are some things to consider when you use options like:
 - Is it optionnal or required ?
 - What is the type of the option ? An user, a number, ... ?
 - Does the option refer to multiple element (ex: voice / text channel)

*Bonus :* You could add an option so we can tell the command what channel we want to delete message from

## Exercice 3
Make two slash commands that can **ban** and **unban** an user

## Exercice 4
When you deal with **administrator actions** you need to be sure that only your staff can use your command.
Go back to the previous exercice and make sure that only member with the right [permissions](https://discordjs.guide/slash-commands/permissions.html#member-permissions) can use your command.

## Exercice 5
Make a **warn** command that send a **private message** to the **user** with the **reason**.
*Bonus :* You could add a way to log every warn in a private channel

## Exercice 6
Go back to the first exercice and **warn** the user when the event is triggered

## Bonus
When an user reach a certain amount of warn it should be kick of the server.

You might need to update your warn command so you can have an easy way to track down the number of warn of each user

