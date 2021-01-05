Giveaways
=========

What are Giveaways?
-------------------

PhatBot was initially built to handle giveways for the Steam Curator group Just Good PC Games (https://justgoocpgames.com). We had been given many keys to giveaway but didn't have a system in place to run it. I didn't want to manage spreadsheets, so a bot was the answer!

How do Giveaways work in PhatBot?
---------------------------------

Giveaways in PhatBot are run in channels in servers. This was done so instead of having people join for every giveaway, they can join giveaways happening in a channel and always be eligible to win!

This means once someone has entered for a giveaway, they are also entered for any future giveaways in that specific channel.


Once a giveaway have started an alert will go out giving people a chance to enter. It will then wait the Giveaway Rate provided when setting up then start giving away games!

If a user has also linked their Steam to PhatBot, if they win a game it will check their list to see if they already own it and if they do it will pick another winner instead.

Once a user wins a game, they are not eligible to win another game in the same giveaway.

If there are no more eligible users but more keys to giveaway, PhatBot will send out a notification encouraging people to enter the giveaway. If no one wins after 2 more attempts the giveaway will automatically end and any remaining keys will be eligible for future giveaways.

How do I enter to win in a giveaway?
------------------------------------

It is very simple! Go to the server running the giveaway and join the channel that the giveaway is occuring in.

Enter the following command to join the giveaway

.. code-block:: none

  !join

How do I leave a giveaway?
--------------------------

One may ask, why would someone not want to win? Well that can happen when a user provides the keys to giveaway but doesn't have the permissions to create a giveaway themselves. So they would want to leave the eligible pool of winners.

Enter the following command to leave the giveaway

.. code-block:: none

  !leave

Adding Keys
-----------

To add keys, you must have the proper permissions first. This is done to prevent those who would add invalid keys and making a community look bad from... Well doing exactly that.

.. code-block:: none

  !addkey

Creating a Giveaway
-------------------

To create a giveaway you must first enter keys into PhatBot so they can be given away. Look at the :ref:`pages/Commands#Giveaway Contributor` documentation for 
