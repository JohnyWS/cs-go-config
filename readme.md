# My CS:GO configs

This repo is my way of tracking settings in CS:GO, and I hope you can find something of use, if not least a way to structure your files, so the whole thing is a bit easier to manage.

## The details

The repo can be cloned directly into your cfg folder (default "`<steam_folder>\userdata\<user_id>\730\local\cfg\`"), but it will then auto-load all my configurations on game load. It will not, however, change your settings permanently, so your config.cfg will remain unharmed!

`autoexec.cfg` has almost no content, and you can easily replace it with your own. It calls my boot cfg which then loads all the default cfg's, with the added touch of running my credits.cfg in the end, which prints out where I collected all my input from.

## Troubleshooting

1) The configs does not load?
   Then you might have overridden what you load on startup. Check your launch settings for CS:GO in steam, and see if another config is loaded instead. Either delete that, or point it to your boot.cfg of choice - in this repo it would be `lib\defaults\kelrond-boot.cfg`.
   Also, when you're at it, consider adding these arguments to the launch settings: `-d3d9ex -console -panorama -novid -high -tickrate 128 -freq 144` (TODO: document them! :smirk: )
