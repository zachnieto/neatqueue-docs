# README

## Introduction

#### [NeatQueue Website](https://www.neatqueue.com)

All NeatQueue commands are slash commands, which means they are invoked using a `/`\
Any Admin command requires the user to have Manage Channels permissions, or have one of the configured NeatQueue staff roles.\
In this documentation, anytime an argument is surrounded by \[square brackets], it is a required argument. If it is surrounded by (parenthesis), it is optional.\
The term MMR stands for Match Making Rating, which corresponds to the hidden rating system used by most competitive games.\
All commands are queue specific unless otherwise stated.

**All stats are tied to the queue name. This means if you create multiple queues with the same queue name, they will share stats.**

Want to Donate? Simply use /donate or visit https://donatebot.io/checkout/505102060119916545

***

## Quick Start

### Starting a Queue

Starting a queue is super simple with NeatQueue, just run one of the following commands:

**`/setup` for an interactive walk through**

**`/startqueue` for a simple default configuration**

**`/load [config_id]` for a specific queue configuration**

**`/globalqueue join [global_queue]` for loading a global configuration and joining the shared leaderboard**

***

## User Commands

### Cancel

#### `/cancel`

**Description**

Start a vote to cancel the current match.

**Usage: `/cancel`**

***

### Compare

#### `/compare`

**Description**

Compare your stats to the given player.

**Usage: `/compare [player2] (player1) (hidden)`**

**Arguments:**

`player2`: _(Required)_ Enter the second user you want to compare to.\
`player1`: _(Optional)_ Enter the first user you want to compare to, or omit for yourself.\
`hidden`: _(Optional)_ If you want the stats to be hidden.

***

### Donate

#### `/donate`

**Description**

Donate to help NeatQueue development.

**Usage: `/donate`**

***

### Force Start

#### `/forcestart`

**Description**

Start a vote to forcestart the game, skips vote if used by staff.

**Usage: `/forcestart`**

***

### Help

#### `/help`

**Description**

View locations where to find help for setup.

**Usage: `/help`**

***

### Info

#### `/info`

**Description**

View information about the queue configuration.

**Usage: `/info`**

***

### Leaderboard

#### `/leaderboard`

**Description**

Shows the leaderboard for the current queue's game.

**Usage: `/leaderboard (page) (type) (queue_name)`**

**Arguments:**

`page`: _(Optional)_ The desired page number.\
`type`: _(Optional)_ The type of leaderboard to display.\
Options: `MMR, Peak MMR, Points, MVPs, Games, Wins, Losses, Winrate, Streak, Peak Streak`\
`queue_name`: _(Optional)_ The queue name to view.

***

### Need

#### `/need`

**Description**

Shows how many players are needed for the queue.

**Usage: `/need (channel)`**

**Arguments:**

`channel`: _(Optional)_ Channel of queue to show need for.

***

### Parties/Teams/Clans/Groups

#### `/party cancelinvites`

**Description**

CAPTAIN ONLY: Cancel all pending invites.

**Usage: `/party cancelinvites [party_name]`**

**Arguments:**

`party_name`: _(Required)_ The party name.

***

#### `/party captain`

**Description**

CAPTAIN ONLY: Designate a new captain if you are the current one.

**Usage: `/party captain [player] [party_name]`**

**Arguments:**

`player`: _(Required)_ The new captain.\
`party_name`: _(Required)_ The team name.

***

#### `/party create`

**Description**

Create a new party.

**Usage: `/party create [party_name]`**

**Arguments:**

`party_name`: _(Required)_ The party name.

***

#### `/party disband`

**Description**

CAPTAIN ONLY: Disband a party.

**Usage: `/party disband [party_name]`**

**Arguments:**

`party_name`: _(Required)_ The party name.

***

#### `/party invite`

**Description**

CAPTAIN ONLY: Invite a new player to the team.

**Usage: `/party invite [player] [party_name]`**

**Arguments:**

`player`: _(Required)_ Player to invite.\
`party_name`: _(Required)_ The party name.

***

#### `/party join`

**Description**

Join a team.

**Usage: `/party join [party_name]`**

**Arguments:**

`party_name`: _(Required)_ The party name.

***

#### `/party kick`

**Description**

CAPTAIN ONLY: Kick a player from the party.

**Usage: `/party kick [player] [party_name]`**

**Arguments:**

`player`: _(Required)_ The player to kick.\
`party_name`: _(Required)_ The team name.

***

#### `/party leave`

**Description**

Leave a team.

**Usage: `/party leave [party_name]`**

**Arguments:**

`party_name`: _(Required)_ The party name.

***

#### `/party list`

**Description**

List your parties.

**Usage: `/party list`**

***

#### `/party selectrole`

**Description**

Specify your role in the team.

**Usage: `/party selectrole [party_name] [role]`**

**Arguments:**

`party_name`: _(Required)_ The party name.\
`role`: _(Required)_ Your role.

***

#### `/party view`

**Description**

View the specified party.

**Usage: `/party view [party_name]`**

**Arguments:**

`party_name`: _(Required)_ The party name.

***

### Ping

#### `/ping`

**Description**

Pings all members in the queue.

**Usage: `/ping`**

***

### Predictions

#### `/predict`

**Description**

Place a bet on the given team for the specified match number.

**Usage: `/predict [gamenumber] [team] [amount]`**

**Arguments:**

`gamenumber`: _(Required)_ Game number of bet on.\
`team`: _(Required)_ Team to place the bet on.\
`amount`: _(Required)_ Amount of points you want to bet.

***

### Register

#### `/register`

**Description**

Initialize your MMR using your account.

**Usage: `/register [account]`**

**Arguments:**

`account`: _(Required)_ Account details.

***

### Require IGN

#### `/ign`

**Description**

Sets your IGN for this queue to help with easy lobby setup.

**Usage: `/ign [ign]`**

**Arguments:**

`ign`: _(Required)_ Your IGN for this queue's platform.

***

### Roles

#### `/role`

**Description**

Set your role.

**Usage: `/role (role)`**

**Arguments:**

`role`: _(Optional)_ Preferred role to use, or omit to remove.

***

### Stats

#### `/stats`

**Description**

Shows your stats.

**Usage: `/stats (hidden) (user) (all_time)`**

**Arguments:**

`hidden`: _(Optional)_ If you want the stats to be hidden.\
`user`: _(Optional)_ The user you want to check stats of.\
`all_time`: _(Optional)_ If you want to view all time stats, only applies to monthly queues.

***

### Substitute

#### `/substitute`

**Description**

Substitute yourself for the given player.

**Usage: `/substitute [player]`**

**Arguments:**

`player`: _(Required)_ Enter the player to replace you.

***

## Admin Commands

### AnonymousQueue / Hiding Names

#### `/anonymousqueue`

**Description**

Sets whether to hide the names of players in queue.

**Usage: `/anonymousqueue [mode]`**

**Arguments:**

`mode`: _(Required)_ Hide players names in queue.\
Options: `Enabled, Disabled`

***

### Anti Cheat

#### `/anticheat channel`

**Description**

Sets the anticheat channel to show flagged users.

**Usage: `/anticheat channel [channel]`**

**Arguments:**

`channel`: _(Required)_ The desired anticheat channel.

***

#### `/anticheat enable`

**Description**

Enable/disable the anticheat system.

**Usage: `/anticheat enable [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Toggle for anticheat.\
Options: `Enabled, Disabled`

***

#### `/anticheat flag incorrectvoting`

**Description**

Set an anticheat trigger for players who vote for the wrong team.

**Usage: `/anticheat flag incorrectvoting [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Flag users who vote wrong.\
Options: `Enabled, Disabled`

***

#### `/anticheat flag newaccount`

**Description**

Set an anticheat trigger for new accounts.

**Usage: `/anticheat flag newaccount [age]`**

**Arguments:**

`age`: _(Required)_ Account age in days.

***

#### `/anticheat flag rejoins`

**Description**

Set an anticheat trigger for if a player rejoins a server.

**Usage: `/anticheat flag rejoins [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Flag users who rejoin the server if they already have stats.\
Options: `Enabled, Disabled`

***

#### `/anticheat flag streak`

**Description**

Set an anticheat trigger for a players streak.

**Usage: `/anticheat flag streak [streak]`**

**Arguments:**

`streak`: _(Required)_ Streak to trigger a flag.

***

#### `/anticheat role`

**Description**

Set a role to assign to flagged players.

**Usage: `/anticheat role [role]`**

**Arguments:**

`role`: _(Required)_ Role to assign.

***

### Auto Ping

#### `/autoping remove`

**Description**

Remove the set auto ping rule.

**Usage: `/autoping remove`**

***

#### `/autoping set`

**Description**

Automatically ping the given role when the queue hits the given size.

**Usage: `/autoping set [role] [size]`**

**Arguments:**

`role`: _(Required)_ Role to ping.\
`size`: _(Required)_ Ping when the queue hits this size.

***

### Balance By

#### `/balanceby roles`

**Description**

Order of role to skill from lowest to highest rated, used if balance by ROLES, not MMR.

**Usage: `/balanceby roles (role1) (role2) (role3) (role4) (role5) (role6) (role7) (role8) (role9) (role10)`**

**Arguments:**

`role1`: _(Optional)_ The role to use in balancing.\
`role2`: _(Optional)_ The role to use in balancing.\
`role3`: _(Optional)_ The role to use in balancing.\
`role4`: _(Optional)_ The role to use in balancing.\
`role5`: _(Optional)_ The role to use in balancing.\
`role6`: _(Optional)_ The role to use in balancing.\
`role7`: _(Optional)_ The role to use in balancing.\
`role8`: _(Optional)_ The role to use in balancing.\
`role9`: _(Optional)_ The role to use in balancing.\
`role10`: _(Optional)_ The role to use in balancing.

***

#### `/balanceby type`

**Description**

(Default: mmr) Sets how teams are balanced.

**Usage: `/balanceby type [mode]`**

**Arguments:**

`mode`: _(Required)_ How teams are balanced.\
Options: `Roles, MMR`

***

### Captain Selection

#### `/captains automute`

**Description**

Automatically mute all non-captains during selection to remove bias.

**Usage: `/captains automute [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If players are muted.\
Options: `Enabled, Disabled`

***

#### `/captains drafttype`

**Description**

Sets the type of draft to either Snake or Straight.

**Usage: `/captains drafttype [type]`**

**Arguments:**

`type`: _(Required)_ The type of draft to use.\
Options: `Snake (1-2-2-2), Straight (1-1-1-1), Hybrid (1-1/2-1-1), Hybrid 2 (1-2-1-1), Vote`

***

#### `/captains role`

**Description**

Sets a role which gets priority for being captain.

**Usage: `/captains role (role)`**

**Arguments:**

`role`: _(Optional)_ The captain role.

***

#### `/captains selection`

**Description**

Choose how captains will be picked.

**Usage: `/captains selection`**

***

### Channel Config

> Due to Discord API limitations, NeatQueue can only update the channel name twice per a 10 minute period.

#### `/channel category`

**Description**

(Default: Parent) Sets whether created channels go in a separate or the parent category.

**Usage: `/channel category [category_mode] (category)`**

**Arguments:**

`category_mode`: _(Required)_ The category setting. If mode is Specified, you must provide the category.\
Options: `Parent, New, Specified`\
`category`: _(Optional)_ The specific category if category\_mode is Specified.

***

#### `/channel name queueempty`

**Description**

Set the channel name when a queue is empty. Can only be updated twice per 10 minutes!.

**Usage: `/channel name queueempty [channel_name]`**

**Arguments:**

`channel_name`: _(Required)_ The channel name.

***

#### `/channel name queuelocked`

**Description**

Set the channel name when a queue is locked. Can only be updated twice per 10 minutes!.

**Usage: `/channel name queuelocked [channel_name]`**

**Arguments:**

`channel_name`: _(Required)_ The channel name.

***

#### `/channel name queuenotempty`

**Description**

Set the channel name when a queue isn't empty. Can only be updated twice per 10 minutes!.

**Usage: `/channel name queuenotempty [channel_name]`**

**Arguments:**

`channel_name`: _(Required)_ The channel name.

***

#### `/channel restrictions`

**Description**

(Default: enabled) Sets whether created channels have restrictions.

**Usage: `/channel restrictions [mode]`**

**Arguments:**

`mode`: _(Required)_ If channels are restricted.\
Options: `Enabled, Disabled`

***

### Clear Queue

#### `/clearqueue`

**Description**

Clears the running queue.

**Usage: `/clearqueue`**

***

### Config Loading/Saving

#### `/load`

**Description**

Loads the queue configuration based on the given name.

**Usage: `/load [config]`**

**Arguments:**

`config`: _(Required)_ Config name.

***

#### `/save`

**Description**

Save the current queue configuration to a name.

**Usage: `/save`**

***

### Cross Chat

#### `/crosschat join`

**Description**

Join/create a crosschat room, to share a text channel between servers.

**Usage: `/crosschat join (room_name) (censored)`**

**Arguments:**

`room_name`: _(Optional)_ Name of the room.\
`censored`: _(Optional)_ If crosschat text should be censored.

***

#### `/crosschat leave`

**Description**

Leave the crosschat.

**Usage: `/crosschat leave`**

***

### Dodge

#### `/dodge autoban`

**Description**

Auto ban players who cause a match to cancel by not joining the voice channel.

**Usage: `/dodge autoban (duration)`**

**Arguments:**

`duration`: _(Optional)_ Duration of time in seconds for the ban to last, or 0 to reset.

***

#### `/dodge mmrpenalty`

**Description**

Deduct MMR from players who dodge the match.

**Usage: `/dodge mmrpenalty [amount]`**

**Arguments:**

`amount`: _(Required)_ Amount of MMR to deduct.

***

#### `/dodge pointspenalty`

**Description**

Deduct points from players who dodge the match.

**Usage: `/dodge pointspenalty [amount]`**

**Arguments:**

`amount`: _(Required)_ Amount of points to deduct.

***

### End Queue

#### `/endqueue`

**Description**

Ends the running queue.

**Usage: `/endqueue`**

***

### Force Start

#### `/forcestartconfig conditions`

**Description**

Sets the requirements for forcestarting.

**Usage: `/forcestartconfig conditions [min_size] (max_size) (only_fair) (auto_start)`**

**Arguments:**

`min_size`: _(Required)_ Enter the minimum number of players required. Set to -1 to disable.\
`max_size`: _(Optional)_ Enter the maximum number of players required. Set to -1 to ignore.\
`only_fair`: _(Optional)_ Should the forcestart happen if teams are not the same size?.\
`auto_start`: _(Optional)_ Should the forcestart vote automatically happen when possible?.

***

#### `/forcestartconfig cooldown`

**Description**

(Default: 300) Sets the forcestart cooldown.

**Usage: `/forcestartconfig cooldown [seconds]`**

**Arguments:**

`seconds`: _(Required)_ Cooldown duration in seconds.

***

### Game Integrations

#### `/requireregister`

**Description**

Specify whether players must register their account before playing.

**Usage: `/requireregister [mode]`**

**Arguments:**

`mode`: _(Required)_ Game to register with, or None to disable.\
Options: `None, Valorant, Rainbow 6, Overwatch, RocketLeague, Custom API, Manually`

> With register mode being Custom API, please check out `https://docs.neatqueue.com/#/?id=webhooks` With register mode Manually, players must have their MMR manually set, either through an admin command or via an API request `https://docs.neatqueue.com/#/?id=endpoints`.

***

### Global Queue

#### `/globalqueue create`

**Description**

Create a global queue. You will not be able to modify certain queue configs after.

**Usage: `/globalqueue create`**

***

#### `/globalqueue join`

**Description**

Join a global queue. You will not be able to modify certain queue configs after.

**Usage: `/globalqueue join [name]`**

**Arguments:**

`name`: _(Required)_ The unique ID of the global queue.

***

#### `/globalqueue leave`

**Description**

Unlink from the global queue.

**Usage: `/globalqueue leave`**

***

### Heroes

#### `/hero add`

**Description**

Adds the given hero.

**Usage: `/hero add [hero_name]`**

**Arguments:**

`hero_name`: _(Required)_ -.

***

#### `/hero bans`

**Description**

Specify the number of hero bans or 0 to disable.

**Usage: `/hero bans [bans] (per_team)`**

**Arguments:**

`bans`: _(Required)_ Number of bans (per team if applicable).\
`per_team`: _(Optional)_ If the hero bans are team by team.

***

#### `/hero remove`

**Description**

Removes the given hero.

**Usage: `/hero remove [hero_name]`**

**Arguments:**

`hero_name`: _(Required)_ The hero to remove, or ALL to remove all.

***

#### `/hero voting`

**Description**

Specify who can vote for hero bans. Defaults to All if no captains.

**Usage: `/hero voting [per_team] [mode]`**

**Arguments:**

`per_team`: _(Required)_ If the map vote goes team by team. Team 1 picks first ban, Team 2 picks next, ...\
`mode`: _(Required)_ Who can vote.\
Options: `All, Captains`

***

### Language

#### `/language`

**Description**

Set the language for the server.

**Usage: `/language [language]`**

**Arguments:**

`language`: _(Required)_ -.\
Options: `English, Spanish, French, Portuguese, Japanese, Russian, German, Italian, Ukrainian, Polish, Hebrew`

***

### Leaderboard Config

> Large servers may benefit from using Text leaderboards since uploading images multiple times a second leads to rate limits for your channel/server. Leaderboard titles are also hyperlinks to the website version of the leaderboard.

#### `/leaderboardconfig edits`

**Description**

Specify who can edit a leaderboard.

**Usage: `/leaderboardconfig edits [edits]`**

**Arguments:**

`edits`: _(Required)_ Who can edit the leaderboard buttons.\
Options: `Staff, Anyone, Creator`

***

#### `/leaderboardconfig ignoreroles add`

**Description**

Will not show players on leaderboard with this role.

**Usage: `/leaderboardconfig ignoreroles add [role]`**

**Arguments:**

`role`: _(Required)_ Required role to show on leaderboard.

***

#### `/leaderboardconfig ignoreroles remove`

**Description**

Remove an ignored leaderboard role.

**Usage: `/leaderboardconfig ignoreroles remove [role]`**

**Arguments:**

`role`: _(Required)_ Role to no longer ignore.

***

#### `/leaderboardconfig monthly`

**Description**

Toggle monthly leaderboards, either resets monthly or rolls over.

**Usage: `/leaderboardconfig monthly [toggle] (mode)`**

**Arguments:**

`toggle`: _(Required)_ If monthly leaderboards are enabled.\
Options: `Enabled, Disabled`\
`mode`: _(Optional)_ If stats reset for the month, or keep rolling.\
Options: `Reset, Rolling`

***

#### `/leaderboardconfig requiredgames`

**Description**

(Default: 1) The required number of games played to be displayed on the leaderboard.

**Usage: `/leaderboardconfig requiredgames [games]`**

**Arguments:**

`games`: _(Required)_ Required number of games.

***

#### `/leaderboardconfig shorturl`

**Description**

Create a short url for leaderboards. Ex: 'MyGame' -> https://www.neatqueue.com/lb/MyGame.

**Usage: `/leaderboardconfig shorturl [url]`**

**Arguments:**

`url`: _(Required)_ Short url for this channel's leaderboard.

***

#### `/leaderboardconfig type`

**Description**

Toggle using the image or text leaderboard.

**Usage: `/leaderboardconfig type [type]`**

**Arguments:**

`type`: _(Required)_ Leaderboard format.\
Options: `Images, Text`

***

### Link Queue

#### `/link`

**Description**

Links the current channel to another channel's queue.

**Usage: `/link [channel]`**

**Arguments:**

`channel`: _(Required)_ Enter the channel to link to.

***

#### `/unlink`

**Description**

Unlinks the current channel.

**Usage: `/unlink`**

***

### Lobby Channel

#### `/lobbychannel automute`

**Description**

If the lobby channel should mute all players.

**Usage: `/lobbychannel automute [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If players are muted in the lobby channel.\
Options: `Enabled, Disabled`

***

#### `/lobbychannel pause`

**Description**

Pause the current lobby channel countdown timer.

**Usage: `/lobbychannel pause`**

***

#### `/lobbychannel pullall`

**Description**

Specify pulling players from all channels when their match starts.

**Usage: `/lobbychannel pullall [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Pull players from all channels.\
Options: `Enabled, Disabled`

***

#### `/lobbychannel returnall`

**Description**

Specify returning players to their original voice channel from before the match.

**Usage: `/lobbychannel returnall [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Return players to their original voice channel.\
Options: `Enabled, Disabled`

***

#### `/lobbychannel set`

**Description**

Specify the channel to move players to/from before/after a game.

**Usage: `/lobbychannel set [channel]`**

**Arguments:**

`channel`: _(Required)_ Channel to drag/drop players from/to.

***

#### `/lobbychannel timer`

**Description**

Specify how long players have to join the voice channel before the match is cancelled.

**Usage: `/lobbychannel timer [timer]`**

**Arguments:**

`timer`: _(Required)_ (Default: 300) Timeout length in seconds.

***

#### `/lobbychannel unpause`

**Description**

Unpause the current lobby channel countdown timer.

**Usage: `/lobbychannel unpause`**

***

### Lobby Details

#### `/lobbydetails location`

**Description**

Sets the lobby details message.

**Usage: `/lobbydetails location [location]`**

**Arguments:**

`location`: _(Required)_ Where to show lobby details.\
Options: `DMs, Teams Message`

***

#### `/lobbydetails remove`

**Description**

Removed the lobby details message.

**Usage: `/lobbydetails remove`**

***

#### `/lobbydetails set`

**Description**

Sets the lobby details message.

**Usage: `/lobbydetails set [message]`**

**Arguments:**

`message`: _(Required)_ Enter the message to send.

> Currently supports five substitutions:
>
> `HOST`: Randomly select a player name\
> `QUEUENUM`: Substitute the queue number\
> `RANDOMTEAM`: Substitute a random team name\
> `RANDOM[Option1,Option2,...]`: Randomly select one of the given options and substitute. Ex: `RANDOM[Heads,Tails]`\
> `PASSWORD#T`: Generate a random string of characters, where # is the length of the password, and T is the type of characters to be in the password. There are currently 5 supported password types:
>
> 1. L: Lowercase Letters only
> 2. U: Uppercase Letters only
> 3. N: Numbers only
> 4. C: Lowercase and Uppercase Letters
> 5. A: Lowercase Letters, Uppercase Letters, and Numbers
>
> Example: `/lobbydetails set "Host: HOST, Lobby Name: QUEUENUM, Lobby Password: PASSWORD8A` could substitute to
>
> "Host: @NeatZ, Lobby Name: 12345, Lobby Password: D83mA76x"
>
> You can further enhance the visuals using Markdown formatting.

***

### Lock

#### `/lock`

**Description**

Lock the queue channel to prevent players from joining.

**Usage: `/lock (all) (auto_lock) (time) (timezone) (repeat)`**

**Arguments:**

`all`: _(Optional)_ Lock all queues?.\
`auto_lock`: _(Optional)_ Automatically lock at the specified time.\
`time`: _(Optional)_ Time to lock at in 24 hour format. Ex: 14:00.\
`timezone`: _(Optional)_ Timezone for the specified time. Defaults to UTC.\
`repeat`: _(Optional)_ Repeat daily or just once.

***

#### `/unlock`

**Description**

Unlock the queue channel to allow players to join.

**Usage: `/unlock (all) (auto_unlock) (time) (timezone) (repeat)`**

**Arguments:**

`all`: _(Optional)_ Unlock all queues?.\
`auto_unlock`: _(Optional)_ Automatically unlock at the specified time.\
`time`: _(Optional)_ Time to unlock at in 24 hour format. Ex: 14:00.\
`timezone`: _(Optional)_ Timezone for the specified time. Defaults to UTC.\
`repeat`: _(Optional)_ Repeat daily or just once.

***

### Logs

#### `/logs`

**Description**

View a log of used NeatQueue commands.

**Usage: `/logs (filter)`**

**Arguments:**

`filter`: _(Optional)_ Filter for logs containing this word.

***

### MMR Change

#### `/mmr ceiling`

**Description**

Sets the highest mmr a player can reach in this queue.

**Usage: `/mmr ceiling (mmr)`**

**Arguments:**

`mmr`: _(Optional)_ Enter the peak rating, or omit to reset.

***

#### `/mmr change allow_disable`

**Description**

Sets if the vote to disable MMR appears.

**Usage: `/mmr change allow_disable [allow_disable]`**

**Arguments:**

`allow_disable`: _(Required)_ If MMR changes should be toggleable.

***

#### `/mmr change hidden`

**Description**

Sets if MMR changes are hidden from players.

**Usage: `/mmr change hidden [hidden]`**

**Arguments:**

`hidden`: _(Required)_ If MMR changes are hidden.

***

#### `/mmr change set`

**Description**

(Default: 50) Sets the MMR change per game.

**Usage: `/mmr change set [amount] (loser_mmr) (static)`**

**Arguments:**

`amount`: _(Required)_ The average MMR change for wins and losses.\
`loser_mmr`: _(Optional)_ Override the MMR change for losses.\
`static`: _(Optional)_ If the MMR change should ALWAYS be this value.

***

#### `/mmr change variance`

**Description**

Sets the variance value. Lower value = higher ranges of MMR changes.

**Usage: `/mmr change variance [amount]`**

**Arguments:**

`amount`: _(Required)_ (Default: 1600) Variance value. See docs for a calculator.

> Calculator: https://www.desmos.com/calculator/3qtwvlrw8q Using the calculator, you can see that as the variance value goes up, the actually outputted MMR change has lower variance.

***

#### `/mmr decay`

**Description**

Enable/disable MMR decay and configure the values.

**Usage: `/mmr decay [toggle] (amount) (duration)`**

**Arguments:**

`toggle`: _(Required)_ Enable/disable MMR decay.\
Options: `Enabled, Disabled`\
`amount`: _(Optional)_ Amount of MMR to decay.\
`duration`: _(Optional)_ After how long should a player decay in seconds.

***

#### `/mmr floor`

**Description**

Sets the lowest mmr a player can reach in this queue.

**Usage: `/mmr floor (mmr)`**

**Arguments:**

`mmr`: _(Optional)_ Enter the lowest rating, or omit to reset.

***

#### `/mmr multipliers placements`

**Description**

Toggle the placement matches multiplier.

**Usage: `/mmr multipliers placements [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If there exists a multiplier for the first 10 matches.\
Options: `Enabled, Disabled`

***

#### `/mmr multipliers remove`

**Description**

Sets the MMR multiplier for the given role.

**Usage: `/mmr multipliers remove [role]`**

**Arguments:**

`role`: _(Required)_ -.

***

#### `/mmr multipliers set`

**Description**

Sets the MMR multiplier for the given role for wins.

**Usage: `/mmr multipliers set [role] [multiplier]`**

**Arguments:**

`role`: _(Required)_ -.\
`multiplier`: _(Required)_ Multiplier value. (Ex: 1.2 for a 20% boost).

***

#### `/mmr multipliers streaks`

**Description**

Toggle the streak multiplier.

**Usage: `/mmr multipliers streaks [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If there exists a multiplier for win/loss streaks.\
Options: `Enabled, Disabled`

***

#### `/mmr requirement`

**Description**

Sets the required mmr to enter this queue.

**Usage: `/mmr requirement (mmr)`**

**Arguments:**

`mmr`: _(Optional)_ Enter the required mmr, or omit to disable.

***

### MVPs

#### `/mvp reward`

**Description**

(Default: 5) MMR reward for MVPs.

**Usage: `/mvp reward [amount]`**

**Arguments:**

`amount`: _(Required)_ Amount of MMR to give as a reward.

***

#### `/mvp toggle`

**Description**

Enable/disable MVP votes for matches.

**Usage: `/mvp toggle [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Enable/disable MVPs.\
Options: `Enabled, Disabled`

***

#### `/mvp voterequired`

**Description**

(Default: Disabled) Require players to vote for MVP before voting for winner.

**Usage: `/mvp voterequired [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If voting for MVP is required.\
Options: `Enabled, Disabled`

***

### Manage Players

#### `/player add`

**Description**

Adds the given player to the queue.

**Usage: `/player add [user] (role) (team)`**

**Arguments:**

`user`: _(Required)_ -.\
`role`: _(Optional)_ Enter the role for the player.\
`team`: _(Optional)_ Enter the team for the player if desired.

***

#### `/player autoban`

**Description**

Auto ban players who cause a match to cancel by not joining the voice channel.

**Usage: `/player autoban (duration)`**

**Arguments:**

`duration`: _(Optional)_ Duration of time in seconds for the ban to last, or 0 to reset.

***

#### `/player ban`

**Description**

Bans a player from queueing for the given duration of time.

**Usage: `/player ban [player] (duration) (reason)`**

**Arguments:**

`player`: _(Required)_ The player to ban.\
`duration`: _(Optional)_ Duration of time in seconds for the ban to last.\
`reason`: _(Optional)_ -.

***

#### `/player banlist`

**Description**

View the player ban list.

**Usage: `/player banlist`**

***

#### `/player remove`

**Description**

Removes the given player from the queue.

**Usage: `/player remove [user]`**

**Arguments:**

`user`: _(Required)_ The player.

***

#### `/player sub`

**Description**

Substitute the first player for the second player.

**Usage: `/player sub [player1] [player2] (gamenum)`**

**Arguments:**

`player1`: _(Required)_ Enter the player to replace.\
`player2`: _(Required)_ Enter the player that will be inserted.\
`gamenum`: _(Optional)_ Game to modify. Can be omitted to use this channels game.

***

#### `/player unban`

**Description**

Unban the given player from queueing.

**Usage: `/player unban [player]`**

**Arguments:**

`player`: _(Required)_ The player to unban.

***

### Maps

#### `/bestof`

**Description**

Sets whether the queue is a best of 3, 5, 7, etc.

**Usage: `/bestof [number] (vote) (voteselection) (eligible_voters)`**

**Arguments:**

`number`: _(Required)_ Best of number.\
`vote`: _(Optional)_ Whether players can vote on the number of matches to play.\
`voteselection`: _(Optional)_ Whether to pick the majority vote, or the lowest voted number.\
Options: `Majority, Lowest`\
`eligible_voters`: _(Optional)_ Who on the team can vote. Defaults to All if no captain selected.\
Options: `All, Captains`

***

#### `/map add`

**Description**

Adds the given map.

**Usage: `/map add [map_name] (game_mode) (image_url)`**

**Arguments:**

`map_name`: _(Required)_ New map name.\
`game_mode`: _(Optional)_ Game mode for map if applicable.\
`image_url`: _(Optional)_ Image to show when map selected.

***

#### `/map bans`

**Description**

Specify the number of map bans per team, or 0 to disable.

**Usage: `/map bans [bans] (per_team)`**

**Arguments:**

`bans`: _(Required)_ Number of bans per team.\
`per_team`: _(Optional)_ If the map bans are team by team.

***

#### `/map remove`

**Description**

Removes the given map.

**Usage: `/map remove [map_name]`**

**Arguments:**

`map_name`: _(Required)_ The map to remove, or ALL to remove all.

***

#### `/map selection`

**Description**

Choose between map votes or always random.

**Usage: `/map selection [map_choice] (gamemode_choice)`**

**Arguments:**

`map_choice`: _(Required)_ Voting, always random, or least common.\
Options: `Vote, Random, Least Frequent`\
`gamemode_choice`: _(Optional)_ Voting, always random, or least common.\
Options: `Vote, Random, Least Frequent`

***

#### `/map voting`

**Description**

Specify who can vote for map picks and map bans. Defaults to All if no captains.

**Usage: `/map voting [per_team] [mode]`**

**Arguments:**

`per_team`: _(Required)_ If the map vote goes team by team. Team 1 picks first map, Team 2 picks next, ...\
`mode`: _(Required)_ Who can vote.\
Options: `All, Captains`

***

### Matchmaking

> The matchmaker works by checking the current queue if there are enough players to create a match. A match will only be created if the total range of player MMRs is less than the specified matchmaking range. Every 15 seconds, the range will be increased by the matchmaking leniency, and the match conditions will be rechecked with this new extended matchmaking range.

#### `/matchmaking leniency`

**Description**

Every 15 seconds, how much the range will increase for a better chance at a match.

**Usage: `/matchmaking leniency [value]`**

**Arguments:**

`value`: _(Required)_ How much to increase the range by.

***

#### `/matchmaking range`

**Description**

The range of MMRs for matches. Tighter range = more waiting and players required.

**Usage: `/matchmaking range [range]`**

**Arguments:**

`range`: _(Required)_ Range of player MMRs.

***

### Migrate Stats

#### `/migratestats`

**Description**

Copies the player stats from the old queue name to the new one.

**Usage: `/migratestats [old_name] [new_name]`**

**Arguments:**

`old_name`: _(Required)_ Old queue name with stats.\
`new_name`: _(Required)_ New name to copy the stats to. Will overwrite any stats stored there.

***

### Miscellaneous/Utility

#### `/misc mention teamscreated`

**Description**

(Default: Disabled) Mention the players after teams are created.

**Usage: `/misc mention teamscreated [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If the players are mentioned after teams are created.\
Options: `Enabled, Disabled`

***

#### `/misc nametype`

**Description**

Sets whether to use nicknames or discord names (Default: nick).

**Usage: `/misc nametype [type]`**

**Arguments:**

`type`: _(Required)_ The type of names to be used.\
Options: `Discord, Nicknames`

***

#### `/misc purge`

**Description**

Delete ALL messages in the channel except the queue message if it exists.

**Usage: `/misc purge`**

***

#### `/misc shuffleonstart`

**Description**

(Default: Disabled) Shuffle the player pool on start.

**Usage: `/misc shuffleonstart [mode]`**

**Arguments:**

`mode`: _(Required)_ -.\
Options: `Disabled, Lottery, Priority`

***

#### `/misc startwhen`

**Description**

(Default: Either) Start the match when the queue fills, or only when forcestarted.

**Usage: `/misc startwhen [mode]`**

**Arguments:**

`mode`: _(Required)_ Condition for starting the match.\
Options: `Queue Filled, Forcestart, Either`

***

### Mod Channel

#### `/staffchannel remove`

**Description**

Remove the set results channel.

**Usage: `/staffchannel remove`**

***

#### `/staffchannel set`

**Description**

Sets the results channel to send queue history.

**Usage: `/staffchannel set [channel] (serverwide)`**

**Arguments:**

`channel`: _(Required)_ The text channel to send queue history to.\
`serverwide`: _(Optional)_ Should the channel be global for all queues or just this one?.

***

### Modify Player Data

#### `/add decaygraceperiod`

**Description**

Add a grace period for a user so they won't be affected by MMR decay.

**Usage: `/add decaygraceperiod [time] (user) (role)`**

**Arguments:**

`time`: _(Required)_ Enter the desired grace period time in seconds.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/add game`

**Description**

Increment the players games, use a negative number to decrement.

**Usage: `/add game (games) (user) (role)`**

**Arguments:**

`games`: _(Optional)_ Enter the desired games to add.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/add loss`

**Description**

Increment the players losses, use a negative number to decrement.

**Usage: `/add loss (losses) (user) (role)`**

**Arguments:**

`losses`: _(Optional)_ Enter the desired losses to add.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/add mmr`

**Description**

Increment the players mmr, use a negative number to decrement.

**Usage: `/add mmr (mmr) (user) (role)`**

**Arguments:**

`mmr`: _(Optional)_ Enter the desired mmr to add.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/add mvps`

**Description**

Increment the players MVPs, use a negative number to decrement.

**Usage: `/add mvps [mvps] (user) (role)`**

**Arguments:**

`mvps`: _(Required)_ Enter the desired MVPs to add.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/add points`

**Description**

Increment the players points (not MMR), use a negative number to decrement.

**Usage: `/add points [points] (user) (role)`**

**Arguments:**

`points`: _(Required)_ Enter the desired points to add.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/add streak`

**Description**

Increment the players streak, use a negative number to decrement.

**Usage: `/add streak (streak) (user) (role)`**

**Arguments:**

`streak`: _(Optional)_ Enter the desired streak to add.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/add win`

**Description**

Increment the players wins, use a negative number to decrement.

**Usage: `/add win (wins) (user) (role)`**

**Arguments:**

`wins`: _(Optional)_ Enter the desired wins to add.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/set games`

**Description**

Sets the players games.

**Usage: `/set games [games] (user) (role)`**

**Arguments:**

`games`: _(Required)_ Enter the desired games.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/set ign`

**Description**

Sets the players IGN (used in `/register` or `/ign`).

**Usage: `/set ign [account] (user) (role)`**

**Arguments:**

`account`: _(Required)_ Enter the desired IGN, or 'none' to remove.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/set losses`

**Description**

Sets the players losses.

**Usage: `/set losses [losses] (user) (role)`**

**Arguments:**

`losses`: _(Required)_ Enter the desired losses.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/set mmr`

**Description**

Sets the players mmr.

**Usage: `/set mmr [mmr] (user) (role)`**

**Arguments:**

`mmr`: _(Required)_ Enter the desired mmr.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/set mvps`

**Description**

Sets the players MVPs.

**Usage: `/set mvps [mvps] (user) (role)`**

**Arguments:**

`mvps`: _(Required)_ The new MVPs amount.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/set points`

**Description**

Sets the players points (not MMR).

**Usage: `/set points [points] (user) (role)`**

**Arguments:**

`points`: _(Required)_ The new points amount.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/set streak`

**Description**

Sets the players streak.

**Usage: `/set streak [streak] (user) (role)`**

**Arguments:**

`streak`: _(Required)_ Enter the desired streak.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

#### `/set wins`

**Description**

Sets the players wins.

**Usage: `/set wins [wins] (user) (role)`**

**Arguments:**

`wins`: _(Required)_ Enter the desired wins.\
`user`: _(Optional)_ The user to modify.\
`role`: _(Optional)_ The role to modify.

***

### Number Of Lobbies

#### `/numberoflobbies`

**Description**

(Default: 1) Sets the number of lobbies to create.

**Usage: `/numberoflobbies [lobbies]`**

**Arguments:**

`lobbies`: _(Required)_ The number of lobbies.

***

### Number Of Teams

#### `/numberofteams`

**Description**

(Default: 2) Sets the number of teams.

**Usage: `/numberofteams [number]`**

**Arguments:**

`number`: _(Required)_ The number of teams.

***

### Party Queue

#### `/partyqueue`

**Description**

Enable party queue, allowing players to create parties with `/party` before joining.

**Usage: `/partyqueue [toggle] (max_size)`**

**Arguments:**

`toggle`: _(Required)_ Enable or disable party queue.\
Options: `Enabled, Disabled`\
`max_size`: _(Optional)_ The max party size.

***

### Predictions

#### `/points change loss`

**Description**

(Default: 100) Set how many points players gain for a loss (not MMR).

**Usage: `/points change loss [value]`**

**Arguments:**

`value`: _(Required)_ Points for a loss.

***

#### `/points change win`

**Description**

(Default: 100) Set how many points players gain for a win (not MMR).

**Usage: `/points change win [value]`**

**Arguments:**

`value`: _(Required)_ Points for a win.

***

#### `/points startingvalue`

**Description**

(Default: 0) Set how many points players start with (not MMR).

**Usage: `/points startingvalue [value]`**

**Arguments:**

`value`: _(Required)_ Starting points value.

***

#### `/predictions channel`

**Description**

Specify the channel to show predictions.

**Usage: `/predictions channel [channel]`**

**Arguments:**

`channel`: _(Required)_ The predictions channel.

***

#### `/predictions role`

**Description**

Role to ping when a prediction opens.

**Usage: `/predictions role [role]`**

**Arguments:**

`role`: _(Required)_ Role to ping.

***

#### `/predictions timer`

**Description**

Specify the duration the prediction lasts before closing.

**Usage: `/predictions timer [timer]`**

**Arguments:**

`timer`: _(Required)_ (Default: 180) Prediction length in seconds.

***

#### `/predictions toggle`

**Description**

Specify the channel to show predictions.

**Usage: `/predictions toggle [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If predictions are enabled or disabled.\
Options: `Enabled, Disabled`

***

### Queue Message

#### `/queuemessage delay`

**Description**

(Default: 3) Sets the delay for when a new queue message comes up.

**Usage: `/queuemessage delay [seconds]`**

**Arguments:**

`seconds`: _(Required)_ New message delay.

***

#### `/queuemessage deletions`

**Description**

(Default: Enabled) Sets whether old queue updates should be deleted.

**Usage: `/queuemessage deletions [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Toggle between editing queue updates, or sending new messages.\
Options: `Enabled, Disabled`

***

#### `/queuemessage edits`

**Description**

(Default: Enabled) Set whether queue updates should edit the previous message.

**Usage: `/queuemessage edits [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Toggle between editing queue updates, or sending new messages.\
Options: `Enabled, Disabled`

***

#### `/queuemessage footer`

**Description**

(Default: None) Set a footer for the queue message.

**Usage: `/queuemessage footer (text) (icon_url)`**

**Arguments:**

`text`: _(Optional)_ Footer contents, or omit to remove.\
`icon_url`: _(Optional)_ -.

***

#### `/queuemessage history`

**Description**

(Default: Disable) Sets whether to send a new message for every queue interaction.

**Usage: `/queuemessage history [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Toggle between sending queue join/leaves in the channel.\
Options: `Enabled, Disabled`

***

#### `/queuemessage image`

**Description**

(Default: None) Set an image for the queue message.

**Usage: `/queuemessage image (image_url)`**

**Arguments:**

`image_url`: _(Optional)_ Direct URL of image, or omit to remove.

***

#### `/queuemessage thumbnail`

**Description**

(Default: None) Set a thumbnail for the queue message.

**Usage: `/queuemessage thumbnail (image_url)`**

**Arguments:**

`image_url`: _(Optional)_ Direct URL of image, or omit to remove.

***

### Queue Name

#### `/queuename`

**Description**

Sets the name for this queue. All stats are tied to the queue name.

**Usage: `/queuename [name]`**

**Arguments:**

`name`: _(Required)_ Enter the queue name.

***

### Queue Type

#### `/queuetype`

**Description**

Select the type of queue to run. See docs for detailed explanations.

**Usage: `/queuetype [type]`**

**Arguments:**

`type`: _(Required)_ The type of queue.\
Options: `PUGs/Normal Individual Queue, Matchmaking, Full Team vs Full Team, Select Team On Join`

> PUGs/Normal Individual Queue: The default queue setup, players join individually to get put into a match when the queue is filled. Matchmaking: Players join the queue, and once there are enough players within their MMR range, a match is created. Full Team vs Full Team: Captains join the queue and pull in the entire team. No team setup is required. Select Team On Join: The queue has join buttons for each team, no team setup is required.

***

### Ranks/Automatically Assign Discord Roles

#### `/autoroles copy`

**Description**

Copies the auto roles config to the desired channel.

**Usage: `/autoroles copy [channel]`**

**Arguments:**

`channel`: _(Required)_ Channel with queue to copy autoroles config to.

***

#### `/autoroles ingame`

**Description**

Assign a role to players who are in a match that is removed after.

**Usage: `/autoroles ingame (role)`**

**Arguments:**

`role`: _(Optional)_ Enter the role, or omit to remove.

***

#### `/autoroles inqueue`

**Description**

Assign a role to players who are in the queue.

**Usage: `/autoroles inqueue (role)`**

**Arguments:**

`role`: _(Optional)_ Enter the role, or omit to remove.

***

#### `/autoroles mmr remove`

**Description**

Removes a condition where player roles are changed based on MMR.

**Usage: `/autoroles mmr remove [role]`**

**Arguments:**

`role`: _(Required)_ Enter the role.

***

#### `/autoroles mmr set`

**Description**

(Ranks) Adds a condition in which player roles are changed based on MMR.

**Usage: `/autoroles mmr set [role] [lower_rating] [upper_rating] (lower_lose_rating) (only_one_allowed)`**

**Arguments:**

`role`: _(Required)_ Enter the role to give/remove.\
`lower_rating`: _(Required)_ The lowest MMR required to gain the role.\
`upper_rating`: _(Required)_ The upper MMR rating to lose the role.\
`lower_lose_rating`: _(Optional)_ (Default: lower\_rating) The MMR the player must fall below to lose the role.\
`only_one_allowed`: _(Optional)_ (Default: True) If this role is assigned, no other MMR autoroles will be allowed.

***

#### `/autoroles refresh`

**Description**

Recalculates all autoroles for players.

**Usage: `/autoroles refresh`**

***

#### `/autoroles topplayers remove`

**Description**

Removes a top player role.

**Usage: `/autoroles topplayers remove [role]`**

**Arguments:**

`role`: _(Required)_ Enter the role.

***

#### `/autoroles topplayers set`

**Description**

Conditionally add/remove a role based on leaderboard position.

**Usage: `/autoroles topplayers set [role] [number]`**

**Arguments:**

`role`: _(Required)_ Enter the role for the top players.\
`number`: _(Required)_ Enter the number of players who can have this role.

***

### Reaction Roles

#### `/reactionroles add`

**Description**

Specify a spectator role which can join any voice channel.

**Usage: `/reactionroles add [channel] [message_id] [role] [reaction] (remove_others) (queue_role)`**

**Arguments:**

`channel`: _(Required)_ Channel where message is.\
`message_id`: _(Required)_ Message to add reaction to.\
`role`: _(Required)_ Role to assign/remove.\
`reaction`: _(Required)_ Reaction that corresponds to this role.\
`remove_others`: _(Optional)_ If the user has this role, remove all other reactionroles in the message they have.\
`queue_role`: _(Optional)_ Option role for `/roles` that the user will default to.

***

### Rematch

#### `/rematches`

**Description**

(Default: true) Toggle the ability to rematch.

**Usage: `/rematches [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If you want rematches to be enabled or disabled.

***

### Requeue

> For queue types that always start when reaching the queue size, requeue priority won't appear to make any changes. However, there are two specific queue starting modes where it will matter:
>
> 1. `/queuetype Matchmaking`: When the matchmaker is running, it will use the overall sum of all player priorities, and use this value to increase the matchmaking range. For example, if the matchmaking range is 300 MMR, but there are two players with 100 priority each, the matchmaking range for that attempted match creation will be 500 MMR, making it more likely for that match to be created. If you want players with priority to ALWAYS be in the match, you can give them a very large priority (like 100,000), which ensures the matchmaker always considers their match as valid.
> 2. `/misc startwhen Forcestarted`: When matches can only be forcestarted, the number of players can exceed the maximum queue size. Players who join the queue with priority will take precedence in the queue over lower priority players.

#### `/requeue condition`

**Description**

Sets the condition for letting a player requeue.

**Usage: `/requeue condition [condition]`**

**Arguments:**

`condition`: _(Required)_ Condition that must be met to requeue.\
Options: `Must Vote, Winner Selected, None`

***

#### `/requeue delay`

**Description**

Delay people from queuing for the given duration after the condition is met.

**Usage: `/requeue delay [seconds]`**

**Arguments:**

`seconds`: _(Required)_ Seconds to delay from queuing.

***

#### `/requeue priority`

**Description**

Give priority to players who requeue after a match.

**Usage: `/requeue priority (value) (seconds)`**

**Arguments:**

`value`: _(Optional)_ (Default: 0) How much priority value to give.\
`seconds`: _(Optional)_ (Default: 300) How many seconds to give this temporary priority value for.

***

#### `/requeue priorityrole add`

**Description**

Allow players with the given role to gain priority for requeue.

**Usage: `/requeue priorityrole add [role] (value)`**

**Arguments:**

`role`: _(Required)_ Priority role.\
`value`: _(Optional)_ (Default: 100) Priority value to assign.

***

#### `/requeue priorityrole remove`

**Description**

Allow players with the given role to gain priority for requeue.

**Usage: `/requeue priorityrole remove [role]`**

**Arguments:**

`role`: _(Required)_ Priority role.

***

### Require IGN

#### `/requireign`

**Description**

(Default: false) Require if players must set their IGN before they can queue.

**Usage: `/requireign [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If you want to require that users set their IGN.\
Options: `Enabled, Disabled`

***

### Required Votes

#### `/requiredvotes`

**Description**

Sets the required votes to pick a winner.

**Usage: `/requiredvotes [type]`**

**Arguments:**

`type`: _(Required)_ The type of voting requirement to be used.\
Options: `Half, Majority, One, Two, Three, Four, Five, Six, Seven, Eight, Nine, Ten`

***

### Requirements

#### `/bannedroles add`

**Description**

Add a banned role which can't join the queue.

**Usage: `/bannedroles add [role]`**

**Arguments:**

`role`: _(Required)_ Enter the banned role.

***

#### `/bannedroles remove`

**Description**

Removed a banned role.

**Usage: `/bannedroles remove [role]`**

**Arguments:**

`role`: _(Required)_ Enter the banned role.

***

#### `/rolerequirement add`

**Description**

Add a required role to enter this queue. Players can join if they have any of the roles.

**Usage: `/rolerequirement add [role]`**

**Arguments:**

`role`: _(Required)_ Enter the required role.

***

#### `/rolerequirement remove`

**Description**

Removed a required role to enter this queue.

**Usage: `/rolerequirement remove [role]`**

**Arguments:**

`role`: _(Required)_ Enter the required role.

***

### Reset Data

#### `/resetstats all`

**Description**

Resets all stats for all queues, or for the inputted queue name.

**Usage: `/resetstats all (queue_name)`**

**Arguments:**

`queue_name`: _(Optional)_ The queue name to reset stats for.

***

#### `/resetstats mmr`

**Description**

Resets all MMR for all queues, or for the inputted queue name.

**Usage: `/resetstats mmr (queue_name)`**

**Arguments:**

`queue_name`: _(Optional)_ The queue name to reset stats for.

***

#### `/resetstats player`

**Description**

Reset the user's data for all queues or a certain queue.

**Usage: `/resetstats player [user] (queue_name)`**

**Arguments:**

`user`: _(Required)_ Enter the desired user.\
`queue_name`: _(Optional)_ Enter the queue data to remove from. Ignore to delete all data from all queues.

***

### Results Channel

#### `/resultschannel`

**Description**

Sets the channel to post match results.

**Usage: `/resultschannel [channel]`**

**Arguments:**

`channel`: _(Required)_ Enter the desired channel.

***

### Roles

#### `/roles`

**Description**

(Default: None) Sets the roles for this queue, or omit to remove all.

**Usage: `/roles (roles) (required)`**

**Arguments:**

`roles`: _(Optional)_ Enter the roles in the form Role,Role,Role,etc.\
`required`: _(Optional)_ If roles are required to be chosen and enforced.

***

### Select Winner

#### `/outcome cancel`

**Description**

Cancel the given game.

**Usage: `/outcome cancel [match_number]`**

**Arguments:**

`match_number`: _(Required)_ The match number.

***

#### `/outcome selectwinner`

**Description**

Sets the winner for the given game.

**Usage: `/outcome selectwinner [match_number] [team_num]`**

**Arguments:**

`match_number`: _(Required)_ The match number.\
`team_num`: _(Required)_ The team that won.

***

#### `/outcome tie`

**Description**

Mark the given game as a tie.

**Usage: `/outcome tie [match_number]`**

**Arguments:**

`match_number`: _(Required)_ The match number.

***

### Server Stats

#### `/serverstats channelnames games`

**Description**

Show how many games have been played by renaming the specified channel.

**Usage: `/serverstats channelnames games (channel) (format)`**

**Arguments:**

`channel`: _(Optional)_ Channel to rename, or omit to remove.\
`format`: _(Optional)_ Format for channel name. Indicate a $ for the replacement. Ex: "Games: $".

***

#### `/serverstats channelnames ingame`

**Description**

Show how many players are in game by renaming the specified channel.

**Usage: `/serverstats channelnames ingame (channel) (format)`**

**Arguments:**

`channel`: _(Optional)_ Channel to rename, or omit to remove.\
`format`: _(Optional)_ Format for channel name. Indicate a $ for the replacement. Ex: "In Game: $".

***

#### `/serverstats channelnames inqueue`

**Description**

Show how many players are in queue by renaming the specified channel.

**Usage: `/serverstats channelnames inqueue (channel) (format)`**

**Arguments:**

`channel`: _(Optional)_ Channel to rename, or omit to remove.\
`format`: _(Optional)_ Format for channel name. Indicate a $ for the replacement. Ex: "In Queue: $".

***

#### `/serverstats channelnames players`

**Description**

Show the total number of players by renaming the specified channel.

**Usage: `/serverstats channelnames players (channel) (format)`**

**Arguments:**

`channel`: _(Optional)_ Channel to rename, or omit to remove.\
`format`: _(Optional)_ Format for channel name. Indicate a $ for the replacement. Ex: "Players: $".

***

#### `/serverstats channelnames users`

**Description**

Show how many users are in the server by renaming the specified channel.

**Usage: `/serverstats channelnames users (channel) (format)`**

**Arguments:**

`channel`: _(Optional)_ Channel to rename, or omit to remove.\
`format`: _(Optional)_ Format for channel name. Indicate a $ for the replacement. Ex: "Users: $".

***

#### `/serverstats info`

**Description**

View all queue names in the server.

**Usage: `/serverstats info (hidden)`**

**Arguments:**

`hidden`: _(Optional)_ If you want the stats to be hidden.

***

### Setup

#### `/setup`

**Description**

Starts the interactive setup.

**Usage: `/setup`**

***

### Show MMR in Name

#### `/ratinginname format`

**Description**

(Default: '- ($)') Sets the format for ratings in nicknames.

**Usage: `/ratinginname format [format] [location]`**

**Arguments:**

`format`: _(Required)_ How the rating should be formatted. A '$' indicates the player's rating.\
`location`: _(Required)_ -.\
Options: `Prefix, Suffix`

***

#### `/ratinginname queuenames`

**Description**

Sets the queue names to use in retrieving player stats, or omit to reset.

**Usage: `/ratinginname queuenames (names)`**

**Arguments:**

`names`: _(Optional)_ The queue names seperated by ',' to use for inserting ratings into '$' indicators in the format.

***

#### `/ratinginname removeallnicknames`

**Description**

Removes all nicknames from all members.

**Usage: `/ratinginname removeallnicknames`**

***

#### `/ratinginname toggle`

**Description**

Enable or disable showing player MMR in their nickname.

**Usage: `/ratinginname toggle [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If ratings should be shown in name.\
Options: `Enabled, Disabled`

***

### Simulate

#### `/simulate`

**Description**

Simulate the MMR distribution for the current configuration.

**Usage: `/simulate (players) (matches)`**

**Arguments:**

`players`: _(Optional)_ The number of players to simulate.\
`matches`: _(Optional)_ The number of matches to simulate.

***

### Spectator Role

#### `/spectatorrole add`

**Description**

Specify a spectator role which can join any voice channel.

**Usage: `/spectatorrole add [role] (can_speak)`**

**Arguments:**

`role`: _(Required)_ Spectator role.\
`can_speak`: _(Optional)_ Can this role speak in the channel?.

***

#### `/spectatorrole remove`

**Description**

Remove's a spectator role.

**Usage: `/spectatorrole remove [role]`**

**Arguments:**

`role`: _(Required)_ Spectator role.

***

### Staff

#### `/staffrole add`

**Description**

Add a staff role that grants full access to all commands.

**Usage: `/staffrole add [role]`**

**Arguments:**

`role`: _(Required)_ Staff role.

***

#### `/staffrole remove`

**Description**

Remove a staff role that grants full access to all commands.

**Usage: `/staffrole remove [role]`**

**Arguments:**

`role`: _(Required)_ Staff role.

***

### Start From Voice Channel

#### `/startfromvc`

**Description**

Creates a queue using all players in the given channel.

**Usage: `/startfromvc [voice_channel]`**

**Arguments:**

`voice_channel`: _(Required)_ The voice channel to start a queue from.

***

### Start Queue

#### `/startqueue`

**Description**

Starts a queue for the current channel.

**Usage: `/startqueue [queuename] [teamsize] (numberofteams)`**

**Arguments:**

`queuename`: _(Required)_ Enter the queue name.\
`teamsize`: _(Required)_ Enter the team size.\
`numberofteams`: _(Optional)_ Enter the number of teams.

***

### Starting MMR

#### `/startingmmr remove`

**Description**

Removes the starting mmr for the given role.

**Usage: `/startingmmr remove [role]`**

**Arguments:**

`role`: _(Required)_ The role to remove starting MMR from.

***

#### `/startingmmr set`

**Description**

Sets the starting mmr for the given role.

**Usage: `/startingmmr set [mmr] (role)`**

**Arguments:**

`mmr`: _(Required)_ The starting mmr value.\
`role`: _(Optional)_ The role.

***

### Stats

#### `/hidestats`

**Description**

Sets whether stats are forced to be hidden (only shown to the user).

**Usage: `/hidestats [toggle]`**

**Arguments:**

`toggle`: _(Required)_ If you want the stats to be always hidden.

***

#### `/statsbutton`

**Description**

Send a button that allows players to show their stats.

**Usage: `/statsbutton`**

***

### Team Creation

#### `/reshuffle`

**Description**

Sets whether players can reshuffle teams in random selection.

**Usage: `/reshuffle [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Whether reshuffling is enabled or disabled.\
Options: `Enabled, Disabled`

***

#### `/teamselection`

**Description**

Choose how teams will be picked.

**Usage: `/teamselection`**

***

### Team Names

#### `/teamnames captains`

**Description**

If team names should be the captains names, if applicable.

**Usage: `/teamnames captains [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Toggle team names being the captain's names.\
Options: `Enabled, Disabled`

***

#### `/teamnames set`

**Description**

Speicfy the names of each team, or omit for the default behavior..

**Usage: `/teamnames set (team_names)`**

**Arguments:**

`team_names`: _(Optional)_ Comma seperated list of team names. Ex: Team 1,Team 2,...

***

### Team Size

#### `/teamsize`

**Description**

Sets the size for each team.

**Usage: `/teamsize [size]`**

**Arguments:**

`size`: _(Required)_ The team size.

***

### Temporary Setup Channels

#### `/tempchannels`

**Description**

(Default: Enabled) Sets whether to create a temporary text channel for setup.

**Usage: `/tempchannels [mode] (channeltype)`**

**Arguments:**

`mode`: _(Required)_ If the temporary setup channels are enabled.\
Options: `Enabled, Disabled`\
`channeltype`: _(Optional)_ If the new channels should be text channels, or threads of this channel.\
Options: `Text Channels, Threads`

***

### Test

#### `/test`

**Description**

Enables testing mode which allows for duplicate queue joining.

**Usage: `/test`**

***

### Ties

#### `/ties`

**Description**

Sets whether tieing is an option for game outcomes.

**Usage: `/ties [toggle]`**

**Arguments:**

`toggle`: _(Required)_ Whether to show the tie option.

***

### Timers

#### `/timer afk`

**Description**

Toggle kicking players for inactivity.

**Usage: `/timer afk [toggle] (timer)`**

**Arguments:**

`toggle`: _(Required)_ Toggle.\
`timer`: _(Optional)_ Enter the AFK timer in seconds (Default: 3600).

***

#### `/timer matchcleanup`

**Description**

(Default: 5400) Sets the timeout before a running game is finished.

**Usage: `/timer matchcleanup [seconds]`**

**Arguments:**

`seconds`: _(Required)_ Enter the time in SECONDS.

***

#### `/timer queuemessage`

**Description**

(Default: 3) Sets the delay for when a new queue message comes up.

**Usage: `/timer queuemessage [seconds]`**

**Arguments:**

`seconds`: _(Required)_ New message delay.

***

#### `/timer queuereset`

**Description**

(Default: 3600) Sets the time before the queue is reset.

**Usage: `/timer queuereset [seconds]`**

**Arguments:**

`seconds`: _(Required)_ Enter the time in SECONDS.

***

#### `/timer votes`

**Description**

(Default: 60) Sets the timeout for voting menus.

**Usage: `/timer votes [seconds]`**

**Arguments:**

`seconds`: _(Required)_ -.

***

#### `/timer winnervotemessage`

**Description**

(Default: 0) Sets the delay before enabling the winner voting message.

**Usage: `/timer winnervotemessage [seconds]`**

**Arguments:**

`seconds`: _(Required)_ Enter the time in SECONDS.

***

### Tournaments

#### `/tournament create`

**Description**

(BETA) Create a new tournament and shows signup buttons.

**Usage: `/tournament create [name] [team_size] [number_of_teams]`**

**Arguments:**

`name`: _(Required)_ The tournament name, also the name of the queue/stats storage for determining seeding.\
`team_size`: _(Required)_ Number of players of each team.\
`number_of_teams`: _(Required)_ Maximum number of teams that can register.

***

#### `/tournament delete`

**Description**

(BETA) Deletes the tournament.

**Usage: `/tournament delete`**

***

#### `/tournament list`

**Description**

(BETA) List all active tournament.

**Usage: `/tournament list`**

***

#### `/tournament setwinner`

**Description**

(BETA) Sets the winner for a match.

**Usage: `/tournament setwinner [round_number] [match_number] [team_number]`**

**Arguments:**

`round_number`: _(Required)_ -.\
`match_number`: _(Required)_ -.\
`team_number`: _(Required)_ -.\
Options: `1, 2`

***

#### `/tournament start`

**Description**

(BETA) Start the tournament.

**Usage: `/tournament start`**

***

### Voice Channel Mode

#### `/voicechannels mode`

**Description**

(Default: required) Sets whether voice channels are required, optional, or disabled.

**Usage: `/voicechannels mode [mode]`**

**Arguments:**

`mode`: _(Required)_ The type of voice channel setting.\
Options: `Optional, Required, Disabled`

***

#### `/voicechannels moveteam`

**Description**

(Default: required) Sets whether voice channels are required, optional, or disabled.

**Usage: `/voicechannels moveteam [when]`**

**Arguments:**

`when`: _(Required)_ The type of voice channel setting.\
Options: `After All Setup, After Teams Created`

***

### Voting Menu

#### `/votingmenu add`

**Description**

Add a new voting menu.

**Usage: `/votingmenu add [title] [options] [key] [team_voting] (order) (button_colors) (show_numbers) (allow_random) (force_random) (number_of_votes)`**

**Arguments:**

`title`: _(Required)_ (Ex: Vote for the Region) The title for the vote.\
`options`: _(Required)_ (Ex: NA,EU) Comma separated list of options. Ignored if options\_variable exists with values.\
`key`: _(Required)_ (Ex: Region Name) The key for this vote for displaying the result after.\
`team_voting`: _(Required)_ Is the vote once per team, once for all teams, or for a specific team?.\
`order`: _(Optional)_ (Ex: 1) The order for this vote in regard to other votes. Votes will occur in ascending order.\
`button_colors`: _(Optional)_ (Ex: blurple,red) Comma separated list of button colors. Valid options: blurple, gray, green, red.\
`show_numbers`: _(Optional)_ If each option should have a number associated with it when displayed.\
`allow_random`: _(Optional)_ If a 'random' option is included in the vote.\
`force_random`: _(Optional)_ If you want to skip the vote altogether and just pick a random option.\
`number_of_votes`: _(Optional)_ Number of votes per player.

***

#### `/votingmenu remove`

**Description**

Remove the given voting menu.

**Usage: `/votingmenu remove [title_and_order]`**

**Arguments:**

`title_and_order`: _(Required)_ Title and corresponding order of voting menu to delete.

***

### Webhooks

> Webhooks receive information about a match as it is being setup. Currently supported actions are:
>
> * MATCH\_STARTED
> * TEAMS\_CREATED
> * MATCH\_COMPLETED
>
> Additionally, if you have `/requireregister mode: Custom API`, you will receive a webhook with action
>
> * REGISTER\_PLAYER
>
> containing various information about the user, as well as the account they are attempting to register. You must either reply with a json object containing at least a "rating" key (ex: {"rating": 1000}), to specify the rating that the player should be registered with, or any non 200 status response to display to the user.
>
> Examples: https://webhook.site/#!/695c599b-fc6d-4a23-aaee-ce170e355fb3/7051d907-b47b-4b05-acc8-96464fa6c565/1

#### `/webhooks add`

**Description**

Add a new webhook to receive queue information.

**Usage: `/webhooks add [url]`**

**Arguments:**

`url`: _(Required)_ Your webhook url.

***

#### `/webhooks delete`

**Description**

Delete this queue's webhook.

**Usage: `/webhooks delete`**

***

#### `/webhooks generatetoken`

**Description**

Generate an API token for your account.

**Usage: `/webhooks generatetoken`**

***

### Winner Message

#### `/winnermessage format`

**Description**

Sets the format for the winner message.

**Usage: `/winnermessage format [mode]`**

**Arguments:**

`mode`: _(Required)_ Formatting type.\
Options: `Detailed, Simple`

***

#### `/winnermessage pin`

**Description**

Sets whether the message gets pinned.

**Usage: `/winnermessage pin [mode]`**

**Arguments:**

`mode`: _(Required)_ Pin mode.\
Options: `Enabled, Disabled`

***

#### `/winnermessage results`

**Description**

Set who can vote for the result, or if results are fully disabled.

**Usage: `/winnermessage results [value]`**

**Arguments:**

`value`: _(Required)_ Who can vote, or if the match has no outcome.\
Options: `Default, Staff Only, Disabled`

***

#### `/winnermessage sticky`

**Description**

Sets whether the message sticks to the bottom of chat.

**Usage: `/winnermessage sticky [mode]`**

**Arguments:**

`mode`: _(Required)_ Sticky mode.\
Options: `Enabled, Disabled`

***

## API

#### Base URL: `https://api.neatqueue.com/`

#### Generate an API token

#### [View Endpoints](https://api.neatqueue.com/docs)
