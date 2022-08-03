.. _utility:

=========
Utilities
=========

-------------
Misc Commands
-------------

Use the following commands to configure and view various other bits and bobs.

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - /info 
     - ``/info``
     - Brief stats overview of the bot.
   * - /invite
     - ``/help``
     - Display an output of common places to find help with the bot.
   * - /invite
     - ``/invite``
     - Sends you a message with the bot invite.
   * - config list 
     - ``/config``
     - Displays the bots configuration.
   * - clone
     - ``!cb clone #ChannelClone All notifications go in here.``
     - You can use this command to clone a channel and pin the message you specify.
   * - prefix
     - ``!cb prefix -``
     - Using the command like this will change your prefix to ``-``

-----------------------
Purge (Delete) Messages
-----------------------

Sometimes you may wish to clear channels, messages or just messages from specific people to help in the effective
moderation of you server. To accomplish this you can use the following commands.

.. Warning:: You must have **Manage Messages** permissions to run this command!
			 Once run, you will be unable to restore deleted messages.

.. list-table::
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - /purge 
     - ``/purge``
     - Deletes 100 messages in the current channel.
   * - /purge count
     - ``/purge count 25``
     - This would purge 25 messages in the current channel.

.. Warning:: The following commands have no confirmation and will execute when run.

.. list-table:: Creator Purge
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - creators purge 
     - ``!cb creators purge``
     - Removes all manually added creators from announcing.
   * - creators purge 
     - ``!cb creators purge twitch``
     - Removes all manually added creators on Twitch from announcing, works for all platforms.
