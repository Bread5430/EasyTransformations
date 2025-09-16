# Easy Transformations

This mod looks to make both the Cloaca Surprise and the Crystal Delight easier to obtain.

## Justification
Both of these transformations are powerful and fun options to play the game that are gated behind long grinds. While you technically can aquire the necessary items to complete these transformations in any run, doing so is grindy to the point where standard procedure is to use a wish command or run extremely specific builds.

By presenting a less grindly method of aquiring these transformations legitimately, this mod opens up more avenues of play for a more diverse range of builds, and reduces the tedium necessary to enable them.


### Cloaca Surprise
Electric Snail Shell - 200 -> 400 Mollusk Rep

Snail Encrusted Mod - 250 -> 450 Mollusk Rep



### Crystal Delight
Old Recipe: Crystal of Eve, Warm Static, Glitter Grenade MkIII, Gentling Cone

New Recipe: Wild Rice, Warm Static


## Implementation Details

A new Crystal Delight recipe was added via **BRDCrystalDelight.cs**.

Chavvah's Recpie Taught block was overwritten via **Factions.xml**. The only necessary line is the \<waterritual\> tag. Not sure if the other things included will cause compatability issues with other mods that look to alter Chavvah faction behavior.

The Electric Snail Shell's **Item.xml** entry was updated with the new rep value.

The a copy of the snail encrusted mod was created, with the small exception of having 450 rep gain, and inserted via **Mods.xml**. The old snail encrusted mod was removed from spawn population tables by emptying its Tables part in **Mods.xml**. Its unknown if this is still obtainable via **Nacham's ribbon**

