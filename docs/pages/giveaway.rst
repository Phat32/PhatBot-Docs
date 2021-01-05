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

The system was built around Steam Game Keys specifically at first, but it has been expanded to accept plain text as the **Game Name**

.. code-block:: none

  !addkey Game Name | XXXXX-XXXXX-XXXXX

Replace the **Game Name** with the name or Steam ID of the game, and replace **XXXXX-XXXXX-XXXXX** with the actual game key.

For example it can look like this

.. code-block:: none

  !addkey Fall Guys Ultimate Knockout | 12345-67890-12345

or look like this 

.. code-block:: none

  !addkey 1097150 | 12345-67890-12345

At this stage you can also include any DLC Keys that are part of the game by adding them to after the key. You can do this as many times as needed

.. code-block:: none

  !addkey 1097150 | 12345-67890-12345 | 54321-09876-54321
  !addkey 1097150 | 12345-67890-12345 | 54321-09876-54321 | 09876-54321-09876

DLC can also be added after the fact incase you forgot, over looked or obtained later

To do that use the following command

.. code-block:: none

  !adddlc XXXXX-XXXXX-XXXXX | YYYYY-YYYYY-YYYYY

**XXXXX-XXXXX-XXXXX** is the original key added to PhatBot and **YYYYY-YYYYY-YYYYY** is the, well DLC key.

.. code-block:: none

  !adddlc 12345-67890-12345 | 54321-09876-54321

Creating a Giveaway
-------------------

To create a giveaway you must first enter keys into PhatBot so they can be given away. Please do that first before doing this.

To actually make a giveaway, go to the channel you want the giveaway to operate in and run this command

.. code-block:: none

  !addgiveaway Giveaway Name | Days | Hour | Minute | rate

**Giveaway Name** is the name of the giveaway

**Days** is how many days from now will the giveaway run. Set to 0 for today

**Hour** is the hour of the day the giveaway should run at
  Keep in mind PhatBot is in PST. Use !time to get the current time for PhatBot if needed

**Minute** is the minute of the day the giveaway should start

**Rate** is how many minutes between each key is given away

In practice it can look something like This

.. code-block:: none

  !addgiveaway Phats Awesome Giveaway Time | 10 | 12 | 0 | 5

This will create a new giveaway called **Phats Awesome Giveaway Time** that will start in 10 days at 12:00 and giveaway a game every 5 minutes
