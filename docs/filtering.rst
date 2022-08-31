.. _filtering:

=========
Filtering
=========

.. note:: These commands are toggled, if you want to remove something from the list, run the command again.

**CouchBot** has the ability to filter announcements to specific games, stream titles.
This will only allow items mentioned on this list to be announced regardless of what creators you may have added.
An example being if someone played Destiny 2 they would never be announced in the following examples.

.. list-table:: Filter Commands
   :widths: 25 25 50
   :header-rows: 1

   * - Name
     - Example
     - Usage
   * - filter game
     - ``/filter type: game platform: twitch filter_text: World of*``
     - Creates a **Game Filter** on Twitch for any games starting with "World of"
   * - filter title
     - ``/filter type: title platform: twitch filter_text: World of*``
     - Creates a **Stream Title Filter** on Twitch for any titles starting with "World of"
   * - filter list
     - ``/filters page: #``
     - Displays a list of the current applicable filters. Page # is optional, defaults to 1.

.. note:: Want to add wildcards to your filters? Go for it! Adding a game filter of `"*of*"` will announce World of Warcraft, World of Tanks, Anything of Anything! Wildcards can be used in Title filtering too.
