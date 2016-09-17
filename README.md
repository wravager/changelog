# changelog

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

<b>server-side</b>
<i>9/17/2016</i>
