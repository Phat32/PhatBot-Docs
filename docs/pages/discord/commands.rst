Discord Commands
================

General
-------

**!time**
  Displays the current time for PhatBot

**!addrole** *role*
  Adds a role to a users profile. This can only add roles below the level of PhatBots own role.
  
  Example:
  
  .. code-block:: none

    !addrole blue

**!removerole** *role*
  Removes the role from the users profile

  Example: 
  
  .. code-block:: none

    !removerole blue

**!roll**
  Rolls a d20

**!roll** *X* d *Y*
  Will roll the *X* number of *Y* type of die

  Example: 
  
  .. code-block:: none

    !roll 2d20

**!roll** *X* d *Y* +/- *Z*
  Will roll the *X* number of *Y* type of die, then do math to the final answer

  Example: 
  
  .. code-block:: none

    !roll 2d20-5

**!waifu**
  Ask PhatBot to be your Waifu. There is a 1 in 10000000 change it will allow it.

**!joke**
  Tells a joke obtained from the `icanhazdadjoke.com API`__

Anime
-----

**!anime** *name*
  Will search for an anime matching the provided name and provide the shows synopsis and various details about the show

  .. code-block:: none

    !anime slime

**!character** *name*
  Will search for an anime character with the provided name and provide a description of the character

  .. code-block:: none

    !character rimuru

Pokemon
-------

**!pokemon**
  Will get a random Pokemon and tell you their description and various stats

**!pokemon** *id*
  Will get the Pokemon and tell you their description and various stats

  .. code-block:: none

    !pokemon 65

**!pokemon** *name*
  Will get the Pokemon and tell you their description and various stats

  .. code-block:: none

    !pokemon Alakazam

Steam
-----

**!steam**
  PhatBot will DM you directions for telling PhatBot what Steam profile is yours

**!mysteam**
  Display your Steam Profile as known by PhatBot

**!game**
  Randomly suggest a game from your library to play

**!game** *@user*
  Randomly suggest a game from the library of the mentioned user

  Example: 
  
  .. code-block:: none

    !game @Phat32#0032

**!recent**
  Show the game you have most recently been playing

**!recent** *@user*
  Show the game the mentioned user has been playing most recently

  Example: 
  
  .. code-block:: none

    !recent @Phat32#0032

**!recent** *X*
  List the X number of most recent games you have played, up to a max of 15

  Example: 
  
  .. code-block:: none

    !recent 10

**!recent** *@user* *X*
  List the X number of most recent games the mentioned user has played, up to a max of 15

  Example: 
  
  .. code-block:: none

    !recent @Phat32#0032 10

**!top**
  Show the game with the most play time on your profile according to Steam

**!top** *X*
  List the top X number of games you have played according to Steam, up to a max of 15

  Example: 
  
  .. code-block:: none

    !top 10

**!top** *@user* *X*
  List the top X number of games for the mentioned user has played according to Steam, up to a max of 15

  Example:

  .. code-block:: none
    
    !top @Phat32#0032 10

**!score** / **!recommended**
  Get the metacritic store and number of recommendations on Steam for the last suggested game provided by **!game**

Giveaway
--------

**!join**
  Enter your name into the giveaway channel. This will enter you to win all giveaways happening in the channel, not just active giveaways.

**!unjoin** / **!leave**
  Remove your name from the giveaway channel. You will still be able to see the messages, but will not be selected to win.

**!giveaway** / **!giveaways**
  Display a list of recent, active, and upcoming giveaways scheduled in the channel

**!keys** / **!keysleft**
  Get a count of the number of keys left in the active giveaway

**!nextgiveaway**
  Get a date a time for the next scheduled giveaway

**!countdown**
  Get a countdown to the next giveaway, as long as they are scheduled to occur within the week

**!games**
  Get DMed a list of the games available in the giveaway

**!mutegiveaway**
  Remove the **Giveaway Alert** role from your profile, muting the notifications

**!alertgiveaway**
  Add the **Giveaway Alert** role to your profile, pinging you when an notification goes out

**!mykeys**
  Get a DM list of the games you have won and the keys for the game

Giveaway Contributor
--------------------

**!addgame** *Name / Steam Store Link / Steam Store ID*
  Add a game to PhatBots knowledgebase. Can profile the Name of the game, the store link, or just the Steam ID of the game

  Example: 
  
  .. code-block:: none

    !addgame Fall Guys Ultimate Knockout
    
    !addgame https://store.steampowered.com/app/1097150/Fall_Guys_Ultimate_Knockout/
    
    !addgame 1097150

**!addkey** *Name* | *Key*
  Add a key to PhatBot to be given away later

  - *Name* - The name of the game the key is for

  - *Key* - The key to be given away

  Example: 
  
  .. code-block:: none

    !addkey Fall Guys Ultimate Knockout | XXXXX-XXXXX-XXXXX

**!addkey** *Steam URL* | *Key*
  Add a key to PhatBot to be given away later

  - *Steam URL* - The URL of the game the key is for from Steam

  - *Key* - The key to be given away

  Example: 
  
  .. code-block:: none

    !addkey https://store.steampowered.com/app/1097150/Fall_Guys_Ultimate_Knockout/ | XXXXX-XXXXX-XXXXX

**!addkey** *Steam ID* | *Key*
  Add a key to PhatBot to be given away later

  - *Steam ID* - The ID of the game the key is for from Steam

  - *Key* - The key to be given away

  Example: 
  
  .. code-block:: none

    !addkey 1097150 | XXXXX-XXXXX-XXXXX

**!addkey** *Name* | *key* | *dlc key*
  Also add DLC to a key in 1 command by adding | *dlc key* to the end. Multiple DLC keys can be added here

  - *DLC Key* - A DLC Key for the game that will be automatically connected to the key being added

  Example: 
  
  .. code-block:: none

    !addkey 1097150 | XXXXX-XXXXX-XXXXX | YYYYY-YYYYY-YYYYY
    
    !addkey 1097150 | XXXXX-XXXXX-XXXXX | YYYYY-YYYYY-YYYYY | ZZZZZ-ZZZZZ-ZZZZZ

**!adddlc** *key* | *dlc key*
  Add a DLC Key to be included with a game that was previously added. Multiple DLC Keys can be added at 1 time

  - *Key* - The key of a game already added to PhatBot

  - *DLC Key* - The key for DLC for the game

  Example: 
  
  .. code-block:: none

    !adddlc XXXXX-XXXXX-XXXXX | YYYYY-YYYYY-YYYYY 
    
    !adddlc XXXXX-XXXXX-XXXXX | YYYYY-YYYYY-YYYYY | ZZZZZ-ZZZZZ-ZZZZZ

**!addgiveaway** *Giveaway Name* | *Days* | *Hour* | *Minute* | *Rate*
  Create a new giveaway. This will include all keys you have added to PhatBot that are unclaimed or not part of an upcoming giveaway

  - *Giveaway Name* - The name of hte giveaway

  - *Days* - The number of days from now you want the giveaway to happen on

  - *Hour* - The hour of the day you want the giveaway to start (all times are PST for the bot)

  - *Minute* - The minute of the hour the giveaway should start

  - *Rate* - How many minutes between each key is given away

  Example: 
  
  .. code-block:: none

    !addgiveaway Phats Awesome Giveaway | 10 | 12 | 0 | 5
    
  This will give you a giveaway named "Phats Awesome Giveaway" that will take place in 10 days, at noon PST, giving away a key every 5 minutes

**!giveawayinterval** *Rate*
  Update the rate the games are given away in an active giveaway

  - *Rate* - The interval in minutes between each game being given away

**!tossin** 
  Add any keys you have added to PhatBot into the current giveaway

**!tossin** *Name*
  Add any keys you have added to PhatBot into the giveaway matching the name provided

  - *Name* - The name of a giveaway you want to add keys too

**!remainingkeys**
  Get a list of Keys you have added that have been been given away

**!claim** *Key*
  Claim a key you have added, removing it from future or current giveaways

  - *Key* - The Key of a game you no longer want to be given away

  Example: 
  
  .. code-block:: none

    !claim XXXXX-XXXXX-XXXXX

**!give** / **!assign** *Key* | (*@User* or *Discord ID*)
  Give a key to a specific user that you have added to PhatBot

  - *Key* - The Key of the game you want to assign
  
  - *User* - Either the @mention of a user or their Discord ID

  Example: 
  
  .. code-block:: none

    !give XXXXX-XXXXX-XXXXX | @Phat32#0032
    
    !give XXXXX-XXXXX-XXXXX | 157694248504918016

**!takeback** / **!unwin** *Game Name* | *@User*
  Take back a game that was assigned to or won by someone. They are still DMed the Key if won in a giveaway, so be careful.

  - *Game Name* - The name of the game to take back a key from
  
  - *@User* - The @ mention of the user to take the key from

  Example: 
  
  .. code-block:: none

    !unwin Fall Guys Fall Guys Ultimate Knockout | @Phat32#0032

Twitch
------

**!twitch**
  Get a DM with a code to DM to PhatBot on Twitch to connect your Twitch and Discord accounts together for Steam commands in Twitch

**!mutetwitch**
  Remove the **Twitch Alert** role from your profile, muting the notifications of someone going live

**!alerttwitch**
  Add the **Twitch Alert** role to your profile, pinging you when someone goes live

Twitter
-------

**!like** *Tweet*
  Like a provided Tweet

  **Requires Admin Channel**

  - *Tweet* - The URL of the tweet to be liked

  Example:

  .. code-block:: none

    !like https://twitter.com/ThePhat32/status/1344951296437075968

Admin
-----

**!ban** *@User*
  Bans the mentioned use from the server

  Example: 
  
  .. code-block:: none

    !ban @Phat32#0032

**!clear** *X*
  Removes the X number of messages sent in the channel

  Example: 
  
  .. code-block:: none

    !clear 10

**!bot**
  Enabled PhatBot to recivie commands in the channel

**!unbot**
  Disabled PhatBot from reciving commands in the channel

**!isadmin**
  Enable the channel to accept Admin Channel commands

**!isnotadmin**
  Removes the ability to issue Admin Channel commands

**!isgiveaway**
  Enabled giveaways to be run in a channel

**!isnotgiveaway**
  Removes the ability to run giveaways in the channel

**!endgiveaway**
  Ends any active giveaways in the channel

**!enabletwitch**
  Creates the **Twitch Alert** role and assigns it to all members of the Discord and will automatically assign it to anyone joining. May need to be run several times in large population servers to assign it to everyone

**!settwitch** *twitch*
  Configures a channel to be connected to a Twitch channel to relay the chat

  Example: 
  
  .. code-block:: none

    !settwich Phat32

**!disabletwitch**
  Disconnects a channel from the connected Twitch channel

**!enabletwitch**
  Re-enable a previously established twitch connection

**!setupgiveaway**
  Creates the **Giveaway Alert** role, assigns it to all members of the Discord and will automatically assign it to anyone joining. May need to be run several times in large population servers to assign it to everyone

**!shutuptwitch**
  Disables the auto adding of **Twitch Alert** to new members

**!twitchmute** *message*
  Configure the message said by PhatBot when someone uses !mutetwitch

  - *message* - The message to be displayed when someone uses !mutetwitch

  Example: 
  
  .. code-block:: none

    !twitchmute You got it boss, you won't get the pings anymore

**!twitchalert** *message*
  Configure the message said by PhatBot when someone uses !alerttwitch

  - *message* - The message to be displayed when someone uses !alerttwitch

  Example: 
  
  .. code-block:: none

    !twitchalert Here come the pings! You will always know when someone goes live in this server!

**!giveawaymute** *message*
  Configure the message said by PhatBot when someone uses !mutegiveaway

  - *message* - The message to be displayed when someone uses !mutegiveaway

  Example: 
  
  .. code-block:: none

    !giveawaymute Okay, no more alerts for free games for you I guess

**!giveawayalert** *message*
  Configure the message said by PhatBot when someone uses !alertgiveaway

  - *message* - The message to be displayed when someone uses !alertgiveaway

  Example: 
  
  .. code-block:: none

    !givewayalert You got it boss! Alerts incoming for free games!

**!joindm** *message*
  Configure the message PhatBot DMs when joining the server. This is empty by default.

  - *message* - The message to be DMed to new members

  Example: 
  
  .. code-block:: none

    !joindm Hey! Welcome to the server! Super happy to have you here!

**!runjoindm**
  Get a DM of the join DM that new members will see to verify it looks how you want it to looks

**!enablejoindm**
  Enables the Join DM feature

**!disablejoindm**
  Disables the Join DM feature

**!addreact** @MessageId, @Emote, @Role
  Add a React Role to a message. This role will be assigned to a user if they react to that message with the same emote and removed if they remove the reaction

  Example:

  .. code-block:: none

    !addreact 879904482018873385 :p32Pog: @AwesomeRole

**!removereact** @MessageId, @Emote
    Remove a React Role from a message
  
    Example:
  
    .. code-block:: none
  
      !removereact 879904482018873385 :p32Pog:

**!clearreacts** @MessageId
    Remove all React Roles from a message
  
    Example:
  
    .. code-block:: none
  
      !clearreacts 879904482018873385

.. _joke: https://icanhazdadjoke.com/api

__ joke_