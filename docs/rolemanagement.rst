.. _rolemanagement:

================
Role Assignment
================

**CouchBot** is capible of assigning roles based on specific criteria such as a user joining the server or typing a phrase in Discord.
This provides opportunities such as typing "*I Love Streams*" to get pinged when a creator goes live etc.

.. caution:: If you are assigning roles, make sure the bot is above the role it is supposed to assign.

If you want Discord users to be assigned a role when they join your Discord server then the following commands will do this for you.

.. list-table:: Server Join Commands
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - role join 
     - ``/role join role: @RoleName``
     - Assigns a role when people join your server.
   * - role join reset 
     - ``/role joinnone``
     - Reset the server join role to nothing.

Reaction Roles are also available to use should you find that easier to implement on your server. Instead of typing a command, your users can react to an emoji attached to a message to be assigned / removed from a given role;

.. .. Note:: A *single* reaction message can contain up to **four** reaction roles. Want more than 4? You will need to provide multiple messages.

.. .. list-table:: Reaction Role Commands
..    :widths: 25 25 50
..    :header-rows: 1

..    * - Name
..      - Example
..      - Usage
..    * - rm 
..      - ``!cb rm @Streamer :thumbsup: Please react to get the Streamer role!``
..      - Adds/Removes a role when someone adds a reaction to the :thumbsup: emoji.
..    * - rm 
..      - ``!cb rm @Streamer :thumbsup: @Announcements :loudspeaker: Please react to get the desired role!``
..      - Adds/Removes a role when someone adds a reaction to the :thumbsup: and/or :loudspeaker: emoji.

.. The final role option available is tied to Twitch only and assigns the person who is live an additional role **only when they are live.**
.. Please see :ref:`Twitch Info <twitch>` for further information on this role.
