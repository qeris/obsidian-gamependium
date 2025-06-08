# Spawning Commands

## Spawn Pokémon
Used to spawn a specified Pokémon at the command user's position.
**Usage**`/spawnpokemon <pokemon> [attributes]`
Alias: `/pokespawn`
**Example**
/spawnpokemon abra shiny ability=synchronize

**Note:** the attributes can be arranged in any order, as long as the command has the name of a Pokémon in it. Both of the following commands are valid examples of this.

**Example 1**
/spawnpokemon shiny ability=synchronize abra**Example** 2
/spawnpokemon shiny abra ability=synchronize

# Spawn Pokémon At
Used to spawn a specified Pokémon at the specified coordinates.
**Usage**`/spawnpokemonat <x> <y> <z> <pokemon> [attributes]`
**Example**
/spawnpokemonat ~ ~ ~ abra shiny ability=synchronize

## Spawn All Pokémon
Used to spawn one of every available Pokémon at the command user's position.
> **Warning:** This may slow down the game for low-end computers.
**Usage**`/spawnallpokemon`
**Example**
/spawnallpokemon

## Spawn Pokémon from Spawn Pool
Attempts to force the spawn system to spawn one or more Pokémon around the command user's location. The command may fail to spawn a Pokémon if spawning it would break configured spawn limits. **This command cannot be executed remotely.**
**Usage**`/spawnpokemonfrompool [number]`
**Example**
/spawnpokemonfrompool 10

## Check Spawn
Used to check the spawning chance of Pokémon for a specified rarity at the command user's current exact position.
**Usage**`/checkspawn <rarity>`
**Example**
/checkspawn ultra-rare

## Party Editing/Inspecting Commands
### Give Pokémon
Used to give a specified Pokémon to the command user.
**Usage**`/givepokemon <pokemon> [attributes]`
Alias: `/pokegive`
**Example**
/givepokemon abra shiny ability=synchronize

## Give Pokémon Other
Used to give a specified Pokémon to a specified player.
**Usage**`/givepokemonother <target> <pokemon> [attributes]`
**Example**
/givepokemonother @a abra shiny ability=synchronize

## Take Pokémon
Used to remove a Pokémon from a specified player's party.
**Usage**`/takepokemon <target> <slot>`
**Example**
/takepokemon @p 1

## Pokémon Edit
Used to edit a Pokémon in a specified slot in the command user's party.
**Usage**`/pokemonedit <slot> [pokemon / attributes]`
Alias: `/pokeedit`
**Example**
/pokemonedit 1 abra ability=adaptability nature=adamant

## Pokémon Edit Other
Used to edit a Pokémon in a specified slot of a specified player's party.
**Usage**`/pokemoneditother <target> <slot> [pokemon / attributes]`
Alias: `/pokeeditother`
**Example**
/pokemoneditother Ash_Green123 1 abra ability=adaptability gender=female nature=adamant

## Heal Pokémon
Used to heal a specified player's party.
**Usage**`/healpokemon [target]`
Alias: `/pokeheal`
**Example**
/healpokemon @p

## Teach
Used to teach a specified move to a Pokémon in a specified slot in a specified player's party.
**Usage**`/teach <target> <slot> <move>`
**Example**
/teach @p 1 synchronoise

## Level Up
Used to increase the level of a Pokémon in a specified slot in a specified player's party by 1.
**Usage**`/levelup <target> <slot>`
**Example**
/levelup @p 1

## Friendship
Used to check a Pokémon's friendship level in a specified slot in the command user's party.
**Usage**`/friendship <slot>`
**Example**
/friendship 1

## Held Item
Used to change the held item for a Pokémon in a specified slot in a specified player's party.
**Usage**`/held_item <target> <slot> <item>`
**Example**
/held_item @p 1 cobblemon:choice_band

## Poké Box
Used to send a Pokémon in a specified slot from a specified player's party to the specified box of their PC.
**Usage**`/pokebox <target> <slot> [box]`
**Example**
/pokebox @p 1 1

## Poké Box All
Used to send all Pokémon in a specified from a specified player's party to the specified box of their PC.
**Usage**`/pokeboxall <target> [box]`
**Example**
/pokebox @p 1

## Give Held Item
Used to give a Pokémon from a specified player's party the provided held item.
**Usage**`/held_item <target> <slot> <item>`
**Example**
/pokebox @p 1 cobblemon:shell_bell

# Player Data Editing Commands
## Give All Pokémon
Used to give one of every available Pokémon to the command user. The Pokémon will be sent to the command user's PC.
**Usage**`/giveallpokemon`
**Example**
/giveallpokemon

## Clear Party
Used to completely reset the target's party.
> **Warning:** As of 1.4 this command does not require a confirmation step. Once executed, immediately erases all Pokémon in the target's party.
**Usage**`/clearparty <target>`
**Example**
/clearparty @p

## Clear PC
Used to completely reset the target's pc.
> **Warning:** As of 1.4 this command does not require a confirmation step. Once executed, immediately erases all Pokémon in the target's PC.
**Usage**`/clearpc <target>`
**Example**
/clearpc @p

## Restart Pokémon
Used to completely reset the user's party and PC.
> **Warning:** As of 1.4 this command does not require a confirmation step. Once executed, immediately erases all Pokémon owned by the user.
**Usage**`/pokemonrestart`
Alias: `/pokerestart`
**Example**
/pokemonrestart

## Restart Pokémon Other
Used to completely reset the target's party and PC.
> **Warning:** As of 1.4 this command does not require a confirmation step. Once executed, immediately erases all Pokémon owned by the target.
**Usage**`/pokemonrestartother <target>`
Alias: `/pokerestartother`
**Example**
/pokemonrestartother @p

# UI Accessing Commands
## PC
Used to access the command user's PC.
**Usage**`/pc`
**Example**
/pc

## Open Starter Screen
Displays the starter Pokémon select interface for a specified player.
**Usage**`/openstarterscreen <target>`
**Example**
/openstarterscreen @p

# Battle Commands
## Stop Battle
Used to stop a specified player's current battle.
**Usage**`/stopbattle <target>`
**Example**
/stopbattle @p

## Abandon Multi Team
Used to remove a player from their MultiBattleTeam. Will disband the team if they are the last remaining member.
**Usage**`/abandonmultiteam`
**Example**
/abandonmultiteam

# Pokedex Commands

## Grant Pokedex Entries
Grants the player all pokemon of the provided Pokedex or a specified species and form.
**Usage**`/pokedex grant <player> all <dex>`OR`/pokedex grant <player> only <species> <form>>`
**Example**
/pokedex grant @p all alolaOR
/pokedex grant @p only decidueye hisui

## Revoke Pokedex Entries
Revokes the player of all pokemon of the provided Pokedex or a specified species and form.
**Usage**`/pokedex revoke <player> all <dex>`OR`/pokedex revoke <player> only <species> <form>>`
**Example**
/pokedex revoke @p all alolaOR
/pokedex revoke @p only decidueye hisui

# NPC Commands
**NOTE: NPC's are currently experimental and may not work as intended**
## Spawn NPC
Used to spawn the provided NPC class with the provided skill level on the player.
**Usage**`/spawnnpc <class> <level>`
**Example**
/spawnnpc standard 1

## Spawn NPC At
Used to spawn the provided NPC class with the provided skill level at the given coordinates.
**Usage**`/spawnnpcat <pos> <class> <level>`
**Example**
/spawnnpcat 0 60 0 standard 1

## Delete NPC
Used to delete the NPC you are looking at.
**Usage**`/npcdelete`
**Example**
/npcdelete

## Edit NPC
Opens the NPC editor GUI (experimental).
**Usage**`/npcedit`
**Example**
/npcedit

## Apply Player Texture
Applies the specified player's texture to the NPC you are looking at.
**Usage**`/applyplayertexture <playername>`
**Example**
/applyplayertexture jeb_

# Misc Commands
### Spawn Bedrock Particle
Spawns the provided bedrock particle on the given entity or position. Useful for testing.
**Usage**`/bedrockparticle <effect> <target>`OR`/bedrockparticle <effect> <world> <pos>`**Example**
/bedrockparticle effectname @pOR
/bedrockparticle effectname minecraft:overworld 0 60 0

## Cobblemon Info
Displays current version info
**Usage**`/cobblemon info`
**Example**
/cobblemon info

## Freeze Pokemon
Freezes the pokemon the player is looking at for the provided time.
**Usage**`/freezepokemon [time]`
**Example**
/freezepokemon 600

## Open Dialogue
Opens the provided dialogue on the provided player.
**Usage**`/opendialogue <dialogue> <player>`
**Example**
/opendialogue example @p

## Run Molang Script
Runs the provided Molang script with the provided optional contexts of the player, NPC or Pokemon entity.
**Usage**`/runmolangscript <script> [player] [npc] [pokemon]`
**Example**
/runmolangscript scriptname @p

## Change Pokemon's Eye Height
Temporarily changes the eyeheight of a species in the provided pose. Recall Pokemon after running command, useful for addon devs to test heights without having to reload resourcepacks.
**Usage**`/changeeyeheight <species> <standing|flying|swimming> <eyeheight>`
**Example**
/changeeyeheight abomasnow standing 0.5

## Change Scale and Size
Temporarily updates a species with the provided species scale and optionally hitbox width and height. Recall pokemon after running command, useful for addon devs to test heights without having to reload resourcepacks
**Usage**`/changescaleandsize <species> <scale> [<width> <height>]`
**Example**
/changescaleandsize abomasnow 5

## Change Walk Speed
Temporarily changes a species walk speed. Recall pokemon after running command, useful for addon devs to test heights without having to reload resourcepacks
**Usage**`/changewalkspeed <species> <walkspeed>`
**Example**
/changewalkspeed abomasnow 5