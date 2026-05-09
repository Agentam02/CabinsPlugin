# CabinsPlugin
A Minecraft plugin that allows you to create cabins, similar to mini-games.
The plugin works on 1.16.5–1.20 Paper/Spigot.


# Features
On the first run of the plugin, you need to create a cabins_world world, or later in the plugin's config.yml under the parameter cabins-world: "" specify the world where cabins will appear.
Otherwise, the plugin will not load.

Additional dependencies are required, without them the plugin will also not start:
Dependencies: WorldGuard, WorldEdit
PlaceholderAPI – optional

For the plugin to work correctly, you need to create a separate world where cabins will be created (specify the world in the plugin's config).

Commands
/cabins create [size] [name] – create a cabin

/cabins delete [name] – delete a cabin

/cabins tp [name] – teleport to a cabin

/cabins admin ban/tempban/warn/unban/unwarn/list/info/create/delete/party – admin commands

/cabins party add – add a player to your cabin region

/cabins party remove – remove a player from your cabin region

/cabins list – list your cabins

/cabins info – view information about yourself

/cabins warnlist – view the list of warnings

/cabins version – display the plugin version

/cabins party tptoggle on/off [name] – enable/disable teleportation to a specific cabin (available since plugin version 2.1)

/cabins party tp on/off [name] – teleport to a friend's cabin (available since plugin version 2.1)

/cabins party info [name] – information about members of the cabin region (available since plugin version 2.1)

Permissions
cabins.create – create a cabin

cabins.delete – delete a cabin

cabins.tp – teleport to a cabin

cabins.admin – all admin permissions at once

cabins.admin.ban / .tempban / .warn / .unban / .unwarn / .list / .info / .create / .delete / .party – individual admin permissions

cabins.view.admin – permission to view admin commands

cabins.view.moder – permission to view moderator commands

cabins.partyhave.[amount] – limit how many players can be added to cabins

cabins.have.[size] – set how many cabins a player can create

cabins.size.[size] – set what cabin size players can create

cabins.list – permission to view your own cabin list

cabins.info – permission to view information about yourself

cabins.warnlist – permission to view the warning list

cabins.version – permission to see the plugin version

cabins.party.add – permission to add a player to your region

cabins.party.remove – permission to remove a player from your region

cabins.party.info – permission to view information about cabin region members

cabins.party.tp – permission to teleport to a friend's cabin

cabins.party.tptoggle – permission to enable/disable teleportation to a specific cabin

Some permissions are not even available to operators, so add them to yourself or to groups.

Placeholders
%cabins_player% – how many cabins the player has

%cabins_warnplayer% – how many warnings the player has

%cabins_banplayer% – whether the player is banned from creating cabins (displays &aYes or &cNo)

%cabins_timeban% – how much time remains on the player's ban (displays time; if the ban is permanent, displays permanent)

If placeholders don't show values, restart the server.

Generated files and folders
The plugin generates the following:
config.yml, lang (folder), data (folder), warnings (folder), bans (folder).

data – stores all created cabins.

warnings – stores all warnings given to players.

bans – stores all player bans.

config.yml – plugin config; you can change region flags, worlds, etc.

Inside the lang folder, there are already two default languages: ru.yml and en.yml. You can set the current language in the config (local: "ru").
