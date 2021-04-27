> # NitroSniper

Discord Nitro sniper and Giveaway joiner in Python.

![Screenshot](screenshot.png)

#### Features

* Multiple accounts support to claim on one main account
* Optional Counter for max Nitro activations
* Optional main account sniper to only claim code from alts
* Cooldown for # hour(s) after redeeming # nitro code(s)
* Duplicate code detection
* Optional Giveaway joiner
* Words blacklist and whitelist to join or not giveaway
* DM host with custom message if giveaway won
* Optional Privnote sniper
* Optional custom status
* Optional Invite link sniper
* Optional Counter for max server joined
* Cooldown for # hour(s) after joining # server(s)
* Webhook support with good only mode that report only codes applied and giveaways won.
* Blacklist servers to not join any giveaways on these servers
* Blacklist servers to not snipe anything in it
* Custom delay to join giveaways, servers and DM giveaways host
* Print Nitro type when applied (Classic or Boost)
* Play sound when Nitro sniped (replace sound.mp3 to change the sound)

#### Usage

Edit `settings.json`

``` json5
{"token": "Nz"}
```

You have multiple choices to run the sniper :

- [Deploy on Heroku](https://heroku.com/deploy) (Free 24/7)
    * Deploy
    * Resources -> enable sniper
    * See logs in More -> View logs



- Compile it yourself
  ``` sh
  go mod download
  go build
  ./NitroSniper
  ```



#### How to obtain your token

https://github.com/Tyrrrz/DiscordChatExporter/wiki/Obtaining-Token-and-Channel-IDs#how-to-get-a-user-token

#### Known issues

* `error unmarshalling READY event` is not a problem, it just happens because you're doing a self bot
* `Already purchased` happens when the gift is a Xbox game pass plan, so if you already activated a discord game pass
  code you can't activate it anymore
* It looks like Discord added a security feature where your token change every time but also expire with 2FA, that might
  be the reason why the sniper doesn't work after some time or if you get an unauthorized error when sniping Nitro
* Some welcome bots mention giveaways that might cause a false positive
* Privnote sniper makes the program crash sometimes, disable it in settings if that happens to you until I find a
  solution

#### Disclaimer

This is against TOS and can get your account banned, especially if you run multiple instance at the same time and/or
claim too many Nitros in a too short amount of time. Use it at your own risks.

> *If you like my sniper consider putting a star on this repo !*
