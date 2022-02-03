.. _youtube:

=============
YouTube Setup
=============

.. caution:: Please ensure you have read through the :ref:`Basic Config <basicconfig>` before moving to this section
             This avoids issues such as the bot not announcing anyone.

YouTube has the unique ability to indefinently store your Live Streams to VOD as well as upload your own content without the need to be Live at all.
**CouchBot**, in turn, will allow you to announce Live, VOD and/or both to your Discord servers!

.. Important:: To remove a creator, run the command again!


--------------
Live Streaming
--------------

Unlike other platforms, YouTube uses a Channel ID as the unique identifier for links and as such you need to know this when adding a
creator to CouchBot.

.. list-table:: Live Streaming
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - youtube
     - ``!cb youtube "YouTube Creator Name or ID" #discord-channel live``
     - A dropdown will appear. Choose the channel to add or remove. Adds / Removes a creator to your list to announce when Live.
   * - youtube
     - ``!cb youtube "YouTube Creator Name or ID" #discord-channel both``
     - A dropdown will appear. Choose the channel to add or remove. Adds / Removes a creator to your list to announce when Live and/or Published.

----------------
Published Videos
----------------

YouTube is known for it's Video content moreso than the Live content it also offers.
To announce when a creator has uploaded a video you would use the following command;

.. list-table:: Published Videos
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - youtube
     - ``!cb youtube "YouTube Creator Name or ID" #discord-channel vod``
     - A dropdown will appear. Choose the channel to add or remove. Adds / Removes a creator to your list to announce when a video is published.
   * - youtube
     - ``!cb youtube "YouTube Creator Name or ID" #discord-channel both``
     -A dropdown will appear. Choose the channel to add or remove.  Adds / Removes a creator to your list to announce when Live and/or Published.
