# UoA Minecraft 2022 Semester 1

Server Manifest

## Timeline

-   5/12/2021 12:58pm - Previous MC server stopped (1.17.1 UoA 2021 S2)
-   5/12/2021 3:12pm - Started on vanilla 1.18
-   26/12/2021 4:24pm - Updated to Paper #101 (1.18.1)
-   6/1/2022 10:29pm - Updated to Paper #134 and added CustomCombat plugin.
-   8/1/2022 9:45pm - Updated to Paper #140, Terralith 2.0.10 and added FAWE plugin and ExplosionRebuilder datapack.
-   27/1/2022 10:20pm - Updated to Paper #176, Core Protect 20.4, Terralith 2.0.12, Server Backup 2.5.1, and installed plugins ProtocolLib (a dependency of) and MCSpells.
-   5/3/2022 7:05pm - Updated to Paper #225 (1.18.2), Terralith 2.1.1a, Simple TPA 5.8, TabTPS 1.3.12, LuckPerms 5.4.9 removing MCSpells & ProtocolLib, and disabling FAWE (no 1.18.2 build yet).

## Datapacks

_In Load Order_

1. [Terralith](https://www.planetminecraft.com/data-pack/terralith-overworld-evolved-100-biomes-caves-and-more/) 2.1.1a (seed: `164682764006463270`)
2. [Vanilla Tweaks](https://vanillatweaks.net/share#MnSd6g)
    1. Cauldron Concrete 2.0.5
    2. Double Shulker Shells 1.3.2
    3. Player Head Drops 1.1.2
    4. Spectator Night Vision 1.1.2
3. [Explosion Rebuilder](https://www.planetminecraft.com/data-pack/repairing-creeper-holes/) 2.0

## Plugins

1.  [SimpleTPA](https://www.spigotmc.org/resources/simple-tpa.64270/) 5.8
2.  [TabTPS](https://www.spigotmc.org/resources/tabtps-1-8-8-1-18-show-tps-mspt-and-more-in-the-tab-menu.82528/) 1.3.12
3.  [CoreProtect](https://www.spigotmc.org/resources/coreprotect.8631/) 20.4
4.  [DiscordSRV](https://www.spigotmc.org/resources/discordsrv.18494/) 1.24.0
5.  [GWarp](https://www.spigotmc.org/resources/gwarp-warp-home-plugin-1-7-x-1-17-x.56824/) 2.13.02
6.  [Server Backup](https://www.spigotmc.org/resources/world-server-backup-1-8-1-17-x-multithreaded.79320/) 2.5.1
7.  [CustomCombat](https://discord.com/channels/@me/857540797120249896/927440567682605157) 6/1/22
8.  [LuckPerms](https://luckperms.net/download) 5.4.9

###### Installed but not active

8.  [Fast Async World Edit (FAWE)](https://ci.athion.net/job/FastAsyncWorldEdit-1.17/) Bukkit-2.0.0-SNAPSHOT-57

## Permissions

Managed by LuckPerms. The following permissions are `true` for the `default` group with no expiry or contexts.

-   `bukkit.command.tps`
-   `gwarp.warp`
-   `minecraft.command.seed`
-   `tabtps.ping`
-   `tabtps.ping.others`
-   `tabtps.tps`
-   ~~`ultimatehomes.sethome.max.2`~~
-   `gwarp.homeamount.2`

## Server Properties

-   [MOTD](https://mctools.org/motd-creator?text=%263UoA+%26a%26lMinecraft+%266%26lServer+%268%2F%2F+%26d%26e1.18.1%21+%0D%0A%26d%26nnachotoast.com%2Fmc)

-   Gamerules
    1. `keepInventory` `true`
    2. `doInsomnia` `false`
    3. `playersSleepingPercentage` `50`
-   Scoreboard Objectives
    -   `health health {"text":"Health", "color": "red"}` - `belowName`
    -   `totalDeaths deathCount` - `list`
    -   `playerDeaths minecraft.killed_by:minecraft.player`
    -   `playerKills playerKillCount`
-   Startup
    ```sh
    java -server -Xmx6656M -Xms5120M -jar *.jar nogui
    ```
