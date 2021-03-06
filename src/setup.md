# Setting Up Rowboat

## Adding the Bot

Join https://discord.gg/rowboat and post your request in the #server-requests channel, following the instructions in the channel topic. Minimum requirement is 1K active users.

## How to Set Up

Once rowboat has been added to your server, go to https://dashboard.rowboat.party/ to edit your server's configuration. Use the sidebar to read about each plugin, then use the example below along with the information in the sidebar to set up your own customized rowboat configuration.

Below is a blank configuration example with web, utilities, admin, modlog, spam, and censor set up. While you can simply copy-paste this to your own server's configuration and fill in the blanks to have a perfectly usable rowboat, it's highly encouraged that you read through the full documentation to understand each component and customize rowboat to your server's needs.

```
web:
  # Username
  ##################: admin
  # Username
  ##################: editor
  # Username
  ##################: viewer

commands:
  overrides: []
  prefix: '!'

levels:
  # Role
  ##################: ###

nickname: R0WB0AT

plugins:

  utilities: {}

  admin:
    mute_role: ##################

  modlog:
    channels:
      #######################:
        exclude: []
        include: []
    ignored_users: []

  spam:
    levels:
      0:
        punishment: TEMPMUTE
        punishment_duration: 120
        max_messages:
          count: 10
          interval: 7
        max_mentions:
          count: 8
          interval: 30
        max_links:
          count: 10
          interval: 60
        max_emojis:
          count: 100
          interval: 120
        max_newlines:
          count: 60
          interval: 120
        max_duplicates:
          count: 5
          interval: 30

  censor:
    levels:
      0:
        filter_invites: true
        invites_whitelist: ['discord-developers', 'discord-testers', 'discord-api', 'events', 'discord-linux', 'gamenight']
        filter_domains: false
        blocked_words: ['word1', 'word2', 'word3']
```
