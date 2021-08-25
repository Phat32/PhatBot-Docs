Twitch Commands
===============

General Commands
----------------

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

.. _joke: https://icanhazdadjoke.com/api

__ joke_

Broadcaster Commands
--------------------

**!sub** Message {$Sub|$Months|$Type}
  Sets the message PhatBot will say when someone Subscribes

  *params*
  $Sub - The name of the subscriber
  $Months - Cumulative count of months subscribed
  $Type - The type of Subscription (Prime, Tier 1, etc)

  Example:
  .. code-block:: none

    !sub $Sub is coming in with a $Type sub! Thank is amazing of you p32O7

**!resub** Message {$Sub|$Months|$Type}
    Sets the message PhatBot will say when someone RE-Subscribes
  
    *params*
    $Sub - The name of the subscriber
    $Months - Cumulative count of months subscribed
    $Type - The type of Subscription (Prime, Tier 1, etc)
  
    Example:
    .. code-block:: none
  
      !resub $Sub is coming in for $Months months with a $Type sub! Thank is amazing of you p32O7