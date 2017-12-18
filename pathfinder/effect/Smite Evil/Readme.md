
# SMITE EVIL

To simulate the Paladin Smite Evil, I have created the following **three** effects. All of these should ideally be set up as ***Actions*** in the character sheet so that they work as intended with the minimum of manual intervention required.

**Effect 1: Standard Smite**

*Target:* Self

*Action:* All

*Effect Text:* `Smite Evil; IFT:ALIGN(evil); ATK: [CHA]; AC: [CHA] deflection; DMG: 5;`

**Effect 2: Bonus Damage vs. Specials**

*Target:* Self

*Action:* Roll

*Effect Text:*	`Smite Special; IFT:TYPE(undead, dragon, outsider); IFT:ALIGN(evil); DMG: 5;`

**Effect 3: Ignore DR**

*Target:* Self

*Action:* All

*Effect Text:*	`Smite DR; DMGTYPE:spell;`

## How to Use
1. Apply Effect 1
2. Apply Effect 2
3. Apply Effect 3
4. Go to Combat Tracker
5. Open Effects list for character
6. Use *Effect Target* option for both effects to target the **Smite Evil** target
7. Ensure that the third effect is only ON when attacking your **Smite Evil** target. This can be toggled in the expanded effects view of the Combat Tracker.

## NOTE:
- The bonus DMG value in these effects is supposed to be equal to a characters Paladin Level. However, Fantasy Grounds does not have any "Level" parameter. As a result, ensuring that the Smite Evil damage value is correct for both effects is something that needs to be updated as part of the Level Up process, and should be checked before using these effects.
- If the target does not have any DR, you can just ignore the third effect. 
- The *spell* damage type has been used in order to simulate the fact that Smite Evil bypasses the DR of evil creatures. I originally had it included in the first  Effect, but unfortunately the DMGTYPE modifier seems to stop working when placed after the IFT:ALIGN(evil) condition for some reason, and also ceases to function once an effect is targetted. If anyone finds an way to make this work. 
