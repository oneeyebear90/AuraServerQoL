Download Aura Server QoL Plugin from these trusted hosts!

[![Modrinth Version](https://img.shields.io/modrinth/v/auraserverqol?style=flat-square&logo=modrinth&label=Modrinth)](https://modrinth.com/plugin/auraserverqol) [![Hangar](https://img.shields.io/badge/Hangar-AuraServerQoL-blue?style=flat-square&logo=paperMC&logoColor=white)](https://hangar.papermc.io/oneeyebear/AuraServerQoL)

Please report any found bugs here on GitHub!

[![GitHub Issues](https://img.shields.io/github/issues/oneeyebear90/AuraServerQoL?style=flat-square&logo=github)](https://github.com/oneeyebear90/AuraServerQoL/issues)

# AuraServerQoL

**AuraServerQoL** is a lightweight, server-side Paper plugin designed to bring essential Quality-of-Life (QoL) features and smooth mechanics to your Minecraft server—**without requiring your players to install any client-side mods!**

---

## 🌟 What Does AuraServerQoL Do?
* **Dynamic Lighting for all: (`/auralights`)** Activated by the player holding a light source such as a torch/lantern/glowstone/etc. in their mainhand or off-hand. Normally a feature that is limited to those clients with loaded shaders or client-side mods. We change that requirement allowing anyone that joins your server to enjoy the feature. Light brightness is equivalent to the held item's light output vanilla value.
 
* **Auto Tool Replacement: (`/auratoolbreak`)** Automatically swaps broken tools with a fresh matching tool or sword from the player's inventory or hotbar so mining, farming, and combat remain seamless.

* **Boat Jumping & Auto-Hurdling:** Improved boat navigation! Automatic Hurdling makes navigating the waters a lot easier. Boats will pull themselves over obstacles like ice/shore banks/lilypads. Additionally, players can manually launch boats over 1-block obstacles by pressing the **Swap Hands Key (F)**. Tunable settings in the config file.

* **Portable Item Disposal:** Open a safe item disposal window by right-clicking on a Lava Bucket, allowing players to permanently purge unwanted junk items from their inventories without dropping items on the ground.

* **Automatic Crop Replanting:** When players right click to harvest crops, the crop is automatically replanted if the player has the seed/crop necessary to replant in their inventory.

* **Farming Earns XP:** Players are awarded with XP when they harvest crops. XP amount is configurable by min and max values, awarded xp is randomized between those values.

* **Container/Chest Sorting: (`/aurasort`)** An item sort button populates in the lower-right inventory slot for chests, barrels, shulker boxes, etc. When clicked the items inside of the chest are consolidated into their maximum stacks and sorted into groups of alike items. The sort items can be placed in the same slot as the sort button so you do not lose an inventory slot because of the button. 

* **Item Salvage:** Sneak and Right-Click any Grindstone to open an Item Salvage interface. Craftable items can be broken down into their recipe ingredients and given back to the player.

* **Mob Shields:** Admins can create Mob Shields allowing for safe areas that mobs are not allowed to enter. Fully customizable in size, location, naming, and entity whitelisting. Use the command to disable/enable, add/delete, specific shields. Whitelisting entities can be set globally and each shield can have it's own optional whitelist to allow specific mobs access (in addition to the primary global whitelist)

---

## 🚀 Why Download AuraServerQoL?

* **100% Vanilla Client Compatible:** Deliver popular modded-style features to your players without forcing players to install Fabric, Forge, or client mods. Bridging the gap for console players or players that just don't know how to install mods.
* **Fully Configurable:** Every module can be toggled or tuned inside `config.yml`. Don't want boat jumping or dynamic lighting on your server? Simply switch them to `false`!
* **Optimized for Paper:** Built asynchronously and thread-safe from the ground up to prevent tick lag, or server performance dips.

---

## 📋 Permissions
- `auraserverqol.lights` - Allows usage of `/auralights` (Default: `true`)
  * Toggle dynamic lighting feature
- `auraserverqol.auratoolbreak` - Allows usage of `/auratoolbreak` (Default: `true`)
  * Toggle tool replacement feature
- `auraserverqol.aurasort` - Allows usage of `/aurasort` (Default: `true`)
  * Toggle the appearance of the item sort button in containers
- `auraserverqol.book` - Allows usage of `/aurabook` (Default: `true`)
  * Gives the player a reference book of AuraServerQoL features and player commands
- `auraserverqol.shield` - Allows usage of `/aurashield` command management (Default: `op`)
  * Create, delete, list, and toggle mob shield zones
  * Create an Aura Mob Shield in this format `/aurashield create <name/id> <radius>`
    * Shield is created at the players location they are standing. Finer editing can be made in shields.yml
- `auraserverqol.admin` - Access to `/auraserverqol <reload|info|update>` and update notifications (Default: `op`)
  * Reload plugin config
