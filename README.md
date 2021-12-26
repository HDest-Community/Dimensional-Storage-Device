## SUPER IMPORTANT
---
The last commit this mod will work fine on is [8b4bd64c91](https://codeberg.org/mc776/hideousdestructor/src/commit/8b4bd64c914083c26d22a06ebc0e019cb6c4fd19).
After that commit, the mod will still run (hopefully for a while), but a full 7mm mag will have an amount of 3030. Same with 7mm clips. **This is only a visual bug**. It will not result in any expoits (that I am aware of). That is because of the new recast 7mm rounds Matt added.

I will not be fixing this. It's not that I can't, it's that I won't. I am not hardcoding fixes anymore. I am not going to constantly patch my mods because of other people's incompetence. If the mod breaks at some point in the future, too bad. I'm done keeping up with Matt's shitty programming practices. If you randomly use a variable for things it's not supposed to be used for, causing all kinds of problems with other code that assumes the variable does what it says on the tin until it suddenly doesn't, you fucking suck.

### Notes
---
- Loadout code is `dsd`.
- Configuration codes are:
	- `cap`: overrides the starting storage capacity.
- Some HDPickup items cannot be inserted into the backpack. That is intentional as there is no way to save some variables, which results in various exploits caused by packing and unpacking an item.
- Each player gets their own storage.
- Order of items is First-In-First-Out. New items are put at the end of the list.
- The device's bulk scales up depending on how full it is, regardless of capacity. Don't ask me how that works or why. I don't know either.
- The device itself does not hold any items. Meaning two different devices will point to the same storage.
- To expand your storage, hold Zoom and Firemode when picking up a DSD to consume the item and gain extra storage