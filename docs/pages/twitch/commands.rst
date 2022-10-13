Twitch Commands
===============

General Commands
----------------

**!commands**
  Get a list of the commands created just for the channel

**!death**
  Get a count of the number of deaths for the current game

**!followage**
  Get the total amount of time following the channel

**!quote**
  Get a random quote from the channels history, or add a number to get a specific quote

  Examples:

  .. code-block:: none

    !quote
    !quote 69

**!topdeaths**
  Show the top 3 death counts and the game attached to them

**!uptime**
  Get the time the stream has currently been active for

**!watchtime**
  Get the total amount of time spent watching the stream

Fun Commands
------------

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

**!joke**
  Tells a joke obtained from the `icanhazdadjoke.com API`__


**!waifu** 
  Check to see if PhatBot will agree to be your Waifu or not (probably not)

.. _joke: https://icanhazdadjoke.com/api

__ joke_

VIP Commands
------------

**These are commands that are accessible to VIPs, Mods and Broadcasters**

**!death+** {number}
  Add to the death counter for the current game being played. Leave blank for adding just 1, or add a number afterwards to add that many if several were missed

  Examples:

  .. code-block:: none

    !death+
    !death+ 5

**!death-** {number}
  Remove a death from the counter for the current game being played. Leave blank for removing just 1, or add a number afterwards to remove that many if several were added in error

  Examples:5

  .. code-block:: none

    !death-
    !death- 5

**!quote+** Quote
  Add a quote to the list of quotes for the channel

  Examples:

  .. code-block:: none

    !quote+ I believe in the you believing in me

Moderator Commands
------------------

**These commands are accessible to Moderators and Broadcasters**

**!setcommand** Command Response
  Create/Update a command unique to the channel. The command must be all 1 word but the Response can be much longer. Multiple Parameters are available to be used in the responses.

  *params*
  
  - $user - The person issuing the command I.E. the viewer
  - $channel - The name of the channel
  - $title - The current title of the stream
  - $game - The current game / category name
  - $randnum - Get a random number between 1 and 100
  - $randuser - Get a random chatter, they must be active
  - $param - Accept the text after the command as input for the command (See Below for example)

  Example:

  .. code-block:: none

    !setcommand vibe Right now $user is vibing at $randnum%

  This creates the command !vibe for the channel

  .. code-block:: none

    !vibe

  Result:

  *Right now PhatBot is vibing at 69%*

  $param Example:

  .. code-block:: none

    !setcommand so Check out @$param over at twitch.tv/$param!

  This creates the command !so for the channel

  .. code-block:: none

    !so PhatBot

  Result:

  *Check out @PhatBot over at twitch.tv/PhatBot!*

**!removecommand** Command
  Removes a created command from the channel

  Example:

  .. code-block:: none

    !removecommand vibe

**!quote-** number
  Remove a quote from the list of quotes for the channel, must provide the number of the quote that is being removed

  Examples:

  .. code-block:: none

    !quote- 2

Broadcaster Commands
--------------------

**These command must be run by you in your chat to work**

**!autoraid**
  Enable/Disable automatic shoutouts when raided. When enabled and raided PhatBot will use the built in Twitch /shoutout command as well as an annoucement

  Example:

  .. code-block:: none

    !autoraid

**!deathmessage**
  Configure the message PhatBot replies with for viewers using the !death command

  *params*

  - $channel - The name of the channel
  - $deaths - The number of deaths for the game
  - $game - The title of the Game

  Example:

  .. code-block:: none

    !deathmessage p32RIP $channel has died $deaths times in $game

**!raidmessage**
  Configure the annoucement that PhatBot uses when raided and autoraid is enabled

  *params*

  - $raider - The name of the channel that raided

  Example:

  .. code-block:: none

    !raider Thank you $raider for the raid! Check them out over at twitch.tv/$raider p32O7

**!sub** message
  Sets the message PhatBot will say when someone Subscribes

  *params*

  - $sub - The name of the subscriber
  - $months - Cumulative count of months subscribed
  - $type - The type of Subscription (Prime, Tier 1, etc)

  Example:

  .. code-block:: none

    !sub $sub is coming in with a $type sub! Thank is amazing of you p32O7

**!resub** message
  Sets the message PhatBot will say when someone Re-Subscribes. If the Sub message is configured and this is left unconfigured PhatBot will use the Sub message as the Re-Sub message.

  *params*

  - $sub - The name of the subscriber
  - $months - Cumulative count of months subscribed
  - $streak - Their current sub streak
  - $type - The type of Subscription (Prime, Tier 1, etc)

  Example:

  .. code-block:: none

    !resub $sub is coming in for $months months with a $type sub! Thank is amazing of you p32O7

**!giftsub** message
  Sets the message PhatBot will say when someone Gift subs

  *params*

  - $sub - The name of the subscriber
  - $months - Cumulative count of months subscribed
  - $type - The type of Subscription (Prime, Tier 1, etc)
  - $gifter - The name of the gifter, if gifted as Anon the name will be displayed as "Anon"

  Example:

  .. code-block:: none

    !giftsub $gifter is handing $sub a $type sub! Thank is amazing of you p32O7

**!communitysub** message
  Sets the message PhatBot will say when someone gives Community Subscriptions

  *params*

  - $gifter - The name of the gifter, if gifted as Anon the name will be displayed as "Anon"
  - $count - The number of subs that were gifted
  - $type - The type of Subscription (Prime, Tier 1, etc)
  

  Example:
  
  .. code-block:: none

    !communitysub $gifter is handing $count $type subs to the chat! Thank is amazing of you p32O7

**!updateping** {On|Enabled|Enable|Yes|True}
  Configure PhatBot to ping in Discord when stream details are updated like the title or game has changed

  Example:

  .. code-block:: none

    !updateping on
    !updateping off

  *Note: PhatBot is specifically looking for On, Enabled, Enable, Yes, and True to activate the alert. Any other value will disable it.*
  