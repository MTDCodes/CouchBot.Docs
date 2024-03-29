.. _examples:

=============
Example Setup
=============

In these scenarios, we have already followed the :ref:`Basic Configuration <basicconfig>` and have the correct :ref:`Permission <troubleshooting>` structure.
We will use ``MattTheDev`` as the streamer account and ``#notification`` as the Discord channel to announce in.

-----------
Scenario 1
-----------

.. admonition:: Scenario 1

   Announcing only the Server Owner going **Live** with an everyone ping.

A lot of people just want a bot to announce them going live. CouchBot can do this!
We start by allowing the bot to announce live streams then adding our creator.
We then tell the bot to ping the everyone role and allow it to do so.

.. code-block:: none

    /allow 
    Choose 'Live' from the drop down
    /twitch creator: MattTheDev channel: #notification message: The Dev is going live @everyone

-----------
Scenario 2
-----------

.. admonition:: Scenario 2

   Announcing people automatically without adding individually.

Rather than adding people manually one by one, you can have the bot automatically pick up people in your server.
This drastically reduces the setup time and eases the setup process for you.
First, you allow the bot to push live announcements then set the default channel.
Then tell it to find anyone with the streaming status and your done!

.. caution:: The streamer has to have the status "Streaming" to be automatically announced.

.. code-block:: none

    /allow 
    Choose 'Live' from the drop down
    /channel live #notification
    /discovery enable

-----------
Scenario 3
-----------

.. admonition:: Scenario 3

   Automatically announce a specific role going live

Let's say you want anyone with the role VIP to be automatically announced. To do this, you would allow
the bot to push Live and tell it the channel it should be posting in.
All that's left to do is tell it what role it should announce as live!

.. caution:: The streamer has to have the status "Streaming" to be automatically announced.

.. code-block:: none

    /allow 
    Choose 'Live' from the drop down
    /channel live #notification
    /discovery enable role: @VIP

-----------
Scenario 4
-----------

.. admonition:: Scenario 4

   Owner announced separately from anyone else

Some servers may with to have the owner or other "VIP" types announced seperatly from the rest.
To accomplish this we allow live then add the streamers as needed specifiying the channel they should be announced in.

.. code-block:: none

    /allow
    Choose 'Live' from the drop down
    /twitch creator: MattTheDev channel: #ownerchannel
    /twitch creator: Jaymei channel: #otherchannel

-----------
Scenario 5
-----------

.. admonition:: Scenario 5

   YouTube VOD and Live announcements to different channels

We start by allowing the bot to push both live and published content. As the commands are a toggle it will respond with the new setting.
We then add the youtube channel using it's "ChannelID_" and specify the channel it should post to along with whether we want it to be 
**Live** or **VOD**.
It is also possible to leave blank for them to go the the same channel or use the argument "both".

.. _ChannelID: https://youtube.com/account_advanced

.. code-block:: none

    /allow
    Choose 'Live' and 'Published' from the drop down
    /youtube creator: Channel Name channel: #livechannel type: live
    Choose the correct channel from the drop down.
    /youtube creator: Channel Name channel: #publishedchannel type: vod
    Choose the correct channel from the drop down.

-----------
Scenario 6
-----------

.. admonition:: Scenario 6

   Owner announced separately from anyone else mentioning different groups with custom messages.

You want to notify @everyone when you go live. You want to notify @Streamer when others go live.
The third command would use the default live announcement message.

.. code-block:: none

    /twitch creator: MattTheDev channel: #BigNotification message: @everyone CouchBot creator **MattTheDev** is now online!
    /twitch creator: Jaymei channel: #notification message: @Streamer Another custom message!
    /twitch creator: EmElle channel: #notification

--------
Messages
--------

You may wish to configure some custom messages with **CouchBot** to let your server know your
live or maybe just to greet a new user. The following commands will show you how!

.. admonition:: Scenario 1

   Setup hello and goodbye messages

.. note:: You can use the arguments **%USER%** and **%RANDOMUSER%**

.. code-block:: none

    /allow
    Choose 'Greetings' and 'Goodbyes' from the drop down
    /channel greetings #channel-name
    /channel goodbyes #channel-name
    /message greeting Your Custom Greeting Message
    /message goodbye Your Custom Goodbye Message

.. admonition:: Scenario 2

   Custom going live message

So you feel like putting something a bit more personable in the messages for your server?
You can use the following;

.. note:: You can use the arguments **%TITLE%, %GAME%, %CHANNEL% or %URL%**

.. code-block:: none

    /message live Your Custom Live Message
    /message published Your Custom VOD Message
