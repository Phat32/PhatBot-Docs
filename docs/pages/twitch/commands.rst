Twitch Commands
===============

General Commands
----------------

**!commands**
  Get a list of the commands created just for the channel

**!followage**
  Get the total amount of time following the channel

**!watchtime**
  Get the total amount of time spent watching the stream

**!uptime**
  Get the time the stream has currently been active for

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

Moderator Commands
------------------

**These commands are accessible to Moderators and Broadcasters**

**!setcommand** Command Response
  Create a new command unique to the channel. The command must be all 1 word but the Response can be much longer. Multiple Parameters are available to be used in the responses.

  *params*
  
  - $user - The person issuing the command I.E. the viewer
  - $channel - The name of the channel
  - $title - The current title of the stream
  - $game - The current game / category name
  - $randnum - Get a random number between 1 and 100
  - $randuser - Get a random chatter, they must be active

  Example:

  .. code-block:: none

    !setcommand vibe Right now $user is vibing at $randnum%

  This creates the command !vibe for the channel

  Result:

  *Right now PhatBot is vibing at 69%*

**!removecommand** Command
  Removes a created command from the channel

  Example:

  .. code-block:: none
    !removecommand vibe

Broadcaster Commands
--------------------

**These command must be run by you in your chat to work**

**!sub** Message {$Sub|$Months|$Type}
  Sets the message PhatBot will say when someone Subscribes

  *params*

  - $Sub - The name of the subscriber
  - $Months - Cumulative count of months subscribed
  - $Type - The type of Subscription (Prime, Tier 1, etc)

  Example:

  .. code-block:: none

    !sub $Sub is coming in with a $Type sub! Thank is amazing of you p32O7

**!resub** Message {$Sub|$Months|$Type}
  Sets the message PhatBot will say when someone Re-Subscribes. If the Sub message is configured and this is left unconfigured PhatBot will use the Sub message as the Re-Sub message.

  *params*

  - $Sub - The name of the subscriber
  - $Months - Cumulative count of months subscribed
  - $Type - The type of Subscription (Prime, Tier 1, etc)

  Example:

  .. code-block:: none

    !resub $Sub is coming in for $Months months with a $Type sub! Thank is amazing of you p32O7

**!giftsub** Message {$Sub|$Months|$Type|$Gifter}
  Sets the message PhatBot will say when someone Gift subs

  *params*

  - $Sub - The name of the subscriber
  - $Months - Cumulative count of months subscribed
  - $Type - The type of Subscription (Prime, Tier 1, etc)
  - $Gifter - The name of the gifter, if gifted as Anon the name will be displayed as "Anon"

  Example:

  .. code-block:: none

    !giftsub $Gifter is handing $Sub a $Type sub! Thank is amazing of you p32O7

**!communitysub** Message {$Gifter|$Count|$Type}
  Sets the message PhatBot will say when someone gives Community Subscriptions

  *params*

  - $Gifter - The name of the gifter, if gifted as Anon the name will be displayed as "Anon"
  - $Count - The number of subs that were gifted
  - $Type - The type of Subscription (Prime, Tier 1, etc)
  

  Example:
  
  .. code-block:: none

    !communitysub $Gifter is handing $Count $Type subs to the chat! Thank is amazing of you p32O7

**!updateping** {On|Enabled|Enable|Yes|True}
  Configure PhatBot to ping in Discord when stream details are updated like the title or game has changed

  Example:

  .. code-block:: none

    !updateping on
    !updateping off

  *Note: PhatBot is specifically looking for On, Enabled, Enable, Yes, and True to activate the alert. Any other value will disable it.*
  