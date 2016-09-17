# changelog

<b>general</b>
<i>9/17/2016</i>
- Added unlock tokens
  - buying tokens:
    - 1 token cost 15 ROBUX
    - 5 tokens cost 75 ROBUX (+1 free token when pruchased)
    - 10 tokens cost 150 ROBUX (+2 free tokens when purchased)
  - daily gifts/lucky draws/challenges/contracts award tokens
- Added expendable products
  - Double experience
    - rewards 2x experience points for a given amount of time
    - time:
      - 1 hour    = 1 token
      - 3 hours   = 2 tokens
      - 9 hours   = 6 tokens
      - 12 hours  = 8 tokens
      - 24 hours  = 16 tokens
      - lifetime  = 1000 ROBUX
        - lifetime is priced high because lvling up rewards tokens
  - Double weapon experience
    - rewards 2x experience points for a given amount of time
    - time:
      - 1 hour    = 1 token
      - 3 hours   = 2 tokens
      - 9 hours   = 6 tokens
      - 12 hours  = 8 tokens
      - 24 hours  = 16 tokens
      - lifetime  = 500 ROBUX
        - lifetime is priced lower because leveling up weapons does not reward tokens
<b>-----------------------------------------------------------------------------------------------</b>
<b>client-side</b>
<i>9/17/2016</i>
- Added crouch and prone camera restrictions
  - Camera cannot point straight down while in crouch and prone
  - Prone has a more heavily restricted camera than crouch
  - Camera automatically goes to min restricted offset when crouching/proneing
- Added supply drop system
  - Supply drops save in stats
  - No data loss possible
  - Supply drops are in diffrernt tiers
    - common
      - cost 1 token to unlock
      - 90% chance of getting a common item
      - 7% chance of getting a rare item
      - 3% chance of getting a legendary item
    - rare
      - cost 5 tokens to unlock
      - 80% chance of getting a common
      - 25% chace of getting a rare
      - 5% chance of getting a legendary
    - legendary
      - cost 15 tokens to unlock
      - 55% chance of getting a common item
      - 35% chance of getting a rare item
      - 10% chance of getting a legendary item
<b>-----------------------------------------------------------------------------------------------</b>
<b>server-side</b>
<i>9/17/2016</i>
- Added ban system
  - only warning have a cool down, 1+ day bans do not
  - types of bans
    - warning tier 1
      - kicked from the server
      - reasons:
        - lag switching
        - high ping for over 3 seconds (still tbd)
    - warning tier 2
      - 15 min ban
      - reasons:
        - spamming chat
        - excessive use of profanity
        - harrassment towards others
    - warning tier 3
      - 30 min ban
      - reasons:
        - breaking warning tiers 1 or 2 withing a 3 day cooldown period
    - 1 day ban
      - reasons:
        - sending unverified request to the server
        - attempting to edit/change parts of the map
        - attempting to add objects/run code to protected places
    - 3 day ban
      - reasons:
        - doing 1 day ban offenses a second time
    - 7 day ban
      - reasons:
        - doing 1 day ban offenses a third time
    - perma ban
      - reasons:
        - doing 1 day ban offenses a fourth time
- Added server-wide notification system
