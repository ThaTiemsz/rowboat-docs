# Utility Plugin

The utility plugin provides a number of useful and fun commands

## Commands

| Name | Description | Default Level | Usage |
|------|-------------|---------------|-------|
| `!cat` | Returns a random image of a cat | Default | `!cat` |
| `!emoji {emoji}` | Returns information on the given emoji | Default | `!emoji :smiley:` |
| `!geoip {ip}` | Searches given IP and returns information on its location | Default | `!geoip 8.8.8.8` |
| `!info {user}` | Returns information on the given user | Default | `!info 232921983317180416` OR `!info @rowboat#0001`|
| `!jumbo {emojis}` | Returns 128x128px images of the given emoji | Default | `!jumbo :cat: :dog: :rabbit:` |
| `!pwnd {email}` | Searches given email on haveibeenpwnd.com and returns results | Default | `!pwnd johndoe@gmail.com` |
| `!random coin` | Flips a coin and returns the result | Default | `!random coin` |
| `!random number [end number] [start number]` | Returns a random number from 0-10 or in a range if specified | Default | `!random number` OR `!random number 50 20` |
| `!r clear` | Clears all of the user's reminders | Default | `!r clear` |
| `!r add {duration} {content}` OR `!remind {duration} {content}` | Adds a reminder. Bot will mention the user after the specified duration with the given message | Default | `!r add 24h update announcements` OR `!remind 24h update announcements` |
| `!search {query}` | Searches for usernames that match given query | Default | `!search b1nzy` |
| `!seen {user}` | Returns the timestamp of when the bot last saw a message from given user | Default | `!seen 232921983317180416` OR `!seen @rowboat#0001` |
| `!server [guild]` | Returns information on the current server or the Server ID if given | Default | `!server` OR `!server 290923757399310337` |
| `!urban {term}` | Searches given term on Urban Dictionary and returns the highest voted definition | Default | `!urban word` |

## Configuration Example

```
utilities: {}
```

There is no further configuration for this plugin.
