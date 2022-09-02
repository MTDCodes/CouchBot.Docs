.. _messages:

==============
Discord Live Setup
==============

.. caution:: THIS IS NEWLY DEPLOYED. THERE MAY BE BUGS. SUBMIT FEEDBACK TO MATT - LETS MAKE THIS THING AWESOME!

**Use the following commands to configure live Discord announcements, like shown below:**

![Screenshot1](img/screenshot1.png)

1. To enable live announcements, first you need to set a Live channel. This will be shared with Discovery announcements.

`/channel live channel: #DiscordChannelToAnnounceIn`

2. Next, you need to enable Discord Live Announcements via the Allow configuration.

`/allow`

3. When the drop down appears, ensure that a green tick is next to Discord Live Announcements. If not, click on it - and click outside the drop down.
4. At this point, you are now good to go. Anytime someone starts streaming via a Voice Channel, an announcement will be made.

**Want to customize the message / embed?! Look no further!**

1. Most of the message preceding the embed AND the embed contents itself are configurable.
2. Type any variation of the command below .. 

`/discordlive`

* `header` will modify #1 in the screenshot.
* `description` will modify #2 in the screenshot.
* `footer` will modify #3 in the screenshot.
* `message` will modify #4 in the screenshot.
* `mention_role` will modify #5 in the screenshot.

![Screenshot2](img/screenshot2.png)

.. caution:: All of the above are OPTIONAL parameters. If you provide an empty option though .. it will reset the setting previously set.

**Want to assign a role when these users go live?**

Easy peasy! Discord live announcements share the live role with Discovery. 

`/role live role: @RoleToAssignOnLive`

.. note:: Unlike normal announcements - as of 9/2/2022 these **will not** be cleaned up when they go offline.