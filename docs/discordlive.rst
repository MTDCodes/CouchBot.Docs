.. _messages:

==============
Discord Live Setup
==============

Use the following commands to configure live Discord announcements, like shown below:

![Alt text](https://couch.bot/images/docs/DiscordLiveAnnouncements.png "Discord Live Announcement")

1. To enable live announcements, first you need to set a Live channel. This will be shared with Discovery announcements.

/channel live channel: #DiscordChannelToAnnounceIn

2. Next, you need to enable Discord Live Announcements via the Allow configuration.

/allow

3. When the drop down appears, ensure that a green tick is next to Discord Live Announcements. If not, click on it - and click outside the drop down.
4. At this point, you are now good to go. Anytime someone starts streaming via a Voice Channel, an announcement will be made.

Want to customize the message / embed?! Look no further!

1. Most of the message preceding the embed AND the embed contents itself are configurable.
2. Type any variation of the command below .. 

/discordlive header: Custom Header description: Custom Description footer: Custom Footer message: Custom Message mention_role: @RoleToAnnounce

* Header will modify #1 in the screenshot.
* Description will modify #2 in the screenshot.
* Footer will modify #3 in the screenshot.
* Message will modify #4 in the screenshot.
* Mention Role will modify #5 in the screenshot.

![Alt text](https://couch.bot/images/docs/CustomizeDiscordLiveAnnouncements.png "Discord Live Announcement")

Want to assign a role when these users go live? 

Easy peasy! Discord live announcements share the live role with Discovery. 

/role live role: @RoleToAssignOnLive

.. note:: Unlike normal announcements - as of 9/2/2022 these **will not** be cleaned up when they go offline.