.. _messages:

==============
Advanced Messages Setup
==============

.. caution:: If you are looking to setup messages per creator then follow the instructions in the :ref:`Custom Announcements <customannouncements>` section.

Use the following commands to configure custom message options and test them.

.. note:: The following variables are available to use in the **Live** and **Published** messages.
.. code-block:: none

    %TITLE% - Name of the Stream
    %GAME% - Not working for YouTube
    %CHANNEL% - Channel Name
    %URL% - Full URL of the Stream

.. note:: The following variables are available to use in the **Greetings** messages.
.. code-block:: none

    %NEWLINE% - Insert a new line.
    %NICKNAME% - Nickname of the person joining. They do not have one though, this will return username on Greetings.
    %RANDOMUSER% - Grab a random username from the server.
    %SERVER% - Name of the server.
    %SERVERID% - ID of the server.
    %TIMESTAMPUTC% - Current Timestamp, in UTC.
    %USER% - Username of the person joining.
    %USERID% - User ID of the person joining.
    
.. note:: The following variables are available to use in the **Goodbye** messages.
.. code-block:: none

    %HOWLONG% - Human readable amount of time they spent on the server, ie: 3 months, 2 days, and 6 hours.
    %JOINDATE% - The date the person leaving originally joined the server.
    %NEWLINE% - Insert a new line.
    %NICKNAME% - Nickname of the person leaving. If they do not have one, will act like %USER%.
    %RANDOMUSER% - Grab a random username from the server.
    %SERVER% - Name of the server.
    %SERVERID% - ID of the server.
    %TIMESTAMPUTC% - Current Timestamp, in UTC.
    %USER% - Username of the person leaving.
    %USERID% - User ID of the person leaving.

+-------------------+---------------------------------------------------------+-----------------------------------------------+
| Name              | Example                                                 | Usage                                         |
+-------------------+---------------------------------------------------------+-----------------------------------------------+
| message live      | ``/message live "Your Custom Live Message"``         | Changes your live message for the server.     |
+-------------------+---------------------------------------------------------+-----------------------------------------------+
| message published | ``/message published "Your Custom VOD Message"``     | Changes your VOD message for the server.      |
+-------------------+---------------------------------------------------------+-----------------------------------------------+
| message offline   | ``/message offline "Your Custom Offline Message"``   | Changes your offline message for the server.  |
+-------------------+---------------------------------------------------------+-----------------------------------------------+
| message greeting  | ``/message greeting "Your Custom Greeting Message"`` | Changes your greeting message for the server. |
+-------------------+---------------------------------------------------------+-----------------------------------------------+
| message goodbye   | ``/message goodbye "Your Custom Goodbye Message"``   | Changes your goodbye message for the server.  |
+-------------------+---------------------------------------------------------+-----------------------------------------------+

If you want to reset your greetings and messages to the default verbiage, use the following commands;

+--------------------+----------------------------------+--------------------------------------------------------+
| Name               | Example                          | Usage                                                  |
+--------------------+----------------------------------+--------------------------------------------------------+
| message live       | ``/message live clear``       | Resets your live message for the server.               |
+--------------------+----------------------------------+--------------------------------------------------------+
| message published  | ``/message published clear``  | Resets your VOD message for the server.                |
+--------------------+----------------------------------+--------------------------------------------------------+
| message offline    | ``/message offline clear``    | Resets your offline message for the server.            |
+--------------------+----------------------------------+--------------------------------------------------------+
| message greeting   | ``/message greeting clear``   | Resets your greeting message for the server.           |
+--------------------+----------------------------------+--------------------------------------------------------+
| message goodbye    | ``/message goodbye clear``    | Resets your goodbye message for the server.            |
+--------------------+----------------------------------+--------------------------------------------------------+
| message offline    | ``/message offline ""``       | Leaves the original announcement post without changes. |
+--------------------+----------------------------------+--------------------------------------------------------+

To have the message outside of the embed blank, use the following;

+-------------------+---------------------------------+--------------------------------------------------------------+
| Name              | Example                         | Usage                                                        |
+-------------------+---------------------------------+--------------------------------------------------------------+
| message live      | ``/message live empty``      | Remove message outside of embed on live stream announcement. |
+-------------------+---------------------------------+--------------------------------------------------------------+
| message published | ``/message published empty`` | Remove message outside of embed on published announcement.   |
+-------------------+---------------------------------+--------------------------------------------------------------+

If you want to test your messages, use the following commands;

+-------------------+----------------------------------------+----------------------------------------------+
| Name              | Example                                | Usage                                        |
+-------------------+----------------------------------------+----------------------------------------------+
| test live         | ``!cb test live #DiscordChannel``      | Tests your live message for the server.      |
+-------------------+----------------------------------------+----------------------------------------------+
| test published    | ``!cb test published #DiscordChannel`` | Tests your VOD message for the server.       |
+-------------------+----------------------------------------+----------------------------------------------+
| test greeting     | ``!cb test greeting``                  | Tests your greeting message for the server.  |
+-------------------+----------------------------------------+----------------------------------------------+
| test goodbye      | ``!cb test goodbye``                   | Tests your goodbye message for the server.   |
+-------------------+----------------------------------------+----------------------------------------------+
