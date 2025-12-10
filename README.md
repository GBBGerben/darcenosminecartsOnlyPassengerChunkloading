# Darceno's Minecarts Only passenger chunk loading

This datapack is a fork of [Darceno's Minecarts](https://modrinth.com/datapack/darcenos-minecarts) that only keeps the passenger chunk loading functionality and is compatible with 1.21.10. This is not tested for any other version.


### Autonomy
Both **minecart with a mob aboard and minecart with chest** will automatically load surrounding chunks if they're on rails, making it possible for them to cross long distances without the need for a player to be near by.

Here's a pig traveling 1000 blocks all by itself:

![Pig loading chunks](./images/pigloadingchunks.gif)


### Only the necessary
This datapack does not affect empty minecarts, naturally generated minecarts with chest, and other minecarts variations. This ensures that farms utilizing minecarts with hoppers, for example, continue to function normally while also keeping the performance impact as low as possible.

## FAQ and Notes
- **Is it still a mod?** No, I have kept only the datapack code when modifying Darceno's Minecarts. 
- **Is it safe to use?** Yes, and it is also totally interchangeable with vanilla worlds. Adding or removing it to an existing world won't cause any problems (but read the last note). The only thing to keep in mind is if you use command blocks with /forceload, as there will be interference with the functions used by this datapack/mod.
- **Does the mod work on multiplayer?** Yes, and as it is originally a datapack, it is 100% serverside, so the client doesn't need to have it installed.
- **Why was the name changed?** CurseForge wouldn't accept it as "Vanilla Plus Minecarts", and it was a very generic name anyways.
- **Also remember** that if you leave a minecart with a chest/minecart with a mob on top of a rail, even if it's stationary, its chunk will still be loaded. If done excessively, this can cause lag, so it's better to avoid leaving them around carelessly.

**Uninstalling**
- After removing the datapack from an existing world or uninstalling the mod, run the command */forceload remove all*. This is just to ensure that no chunks are left loaded (since the mod will no longer be there to automatically unload them).
