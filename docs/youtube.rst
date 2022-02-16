.. _youtube:

=============
YouTube Setup
=============

.. caution:: Please ensure you have read through the :ref:`Basic Config <basicconfig>` before moving to this section
             This avoids issues such as the bot not announcing anyone.

YouTube has the unique ability to indefinently store your Live Streams to VOD as well as upload your own content without the need to be Live at all.
**CouchBot**, in turn, will allow you to announce Live, VOD and/or both to your Discord servers!

.. Important:: To remove a creator, run the command again!

-----------------
YouTube ID Lookup
-----------------

Unlike other platforms, YouTube uses a Channel ID as the unique identifier for links and as such you need to know this when adding a
creator to CouchBot.

.. list-table:: YouTube ID Lookup
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - /youtube lookup
     - ``/youtube lookup Channel Name``
     - A list of channels and their ID / Description will display if valid.

--------------
Live Streaming
--------------

To announce when a creator has started a stream you would use the following command;

.. list-table:: Live Streaming
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - youtube
     - ``!cb youtube "YouTube Creator Name" #discord-channel live``
     - A dropdown will appear. Choose the channel to add or remove. Adds / Removes a creator to your list to announce when Live.
   * - youtube
     - ``!cb youtube "YouTube Creator Name" #discord-channel both``
     - A dropdown will appear. Choose the channel to add or remove. Adds / Removes a creator to your list to announce when Live and/or Published.
   * - youtube
     - ``!cb youtube YouTube Channel ID #discord-channel live``
     - This will bypass the dropdown, and directly add the YouTube Channel, if a valid ID is passed.
   * - youtube
     - ``!cb youtube YouTube Channel ID #discord-channel both``
     - This will bypass the dropdown, and directly add the YouTube Channel, if a valid ID is passed.

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
   * - youtube
     - ``!cb youtube YouTube Channel ID #discord-channel vod``
     - This will bypass the dropdown, and directly add the YouTube Channel, if a valid ID is passed.
   * - youtube
     - ``!cb youtube YouTube Channel ID #discord-channel both``
     - This will bypass the dropdown, and directly add the YouTube Channel, if a valid ID is passed.
