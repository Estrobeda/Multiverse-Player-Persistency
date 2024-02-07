# Multiverse Player Persistency WIP
## Note: this plugin is heavily inspired by Multiverse-Inventory and might end up being a fork of that plugin with extra functionality for persistency.

Adds per world persistency for individual players. 
Using the /mvtp command teleports the player to their last known location in the world they're teleporting to with the inventory they had before they left that world.

commands:
  - /mvpp on/off
      - enables/disables the plugin
  - /mvpp addw [world_name]
    -  adds the world to the list of worlds with persistency enabled.
  - /mvpp remw [world_name]
    -  removes the world from the list of world with persistency enabled.
  - /mvpp addp [portal_name]
    -  adds a portal to the list of portals that should trigger persistent travel to the world, if the world is listed. otherwise has no effect.
  - /mvpp remp [portal_name]
    -  removes the portal from the list (from addp)
  - /mvpp tp [player] [world]
    -  teleports a player to their last known location on the world, or to world spawn/bed if unknown. (mvtp is overridden with this command but this allows for mvpp specific permissions to be set)

Requirements:
Requirement:
  - multiverse-core

optional:
  - multiverse-portals (for portal commands and logic)
  - multiverse-compass-navigation (adds UI for bedrock & java for world travel using a compass, tbd)
    




