# Rage
Barbarians are the most common characters to have **Rage**, but are not the only ones. The Rage spell and monster abilities are similar to a Barbarians rage, and can be modelled in mostly the same way. 

For now I will just look at Rage in both its most common flavours - Core Barbarian, and Unchained Barbarian. Both types of Rage are similar, with slight differences. 

### Rage "Spell Class"

This is pretty simple to replicate with a character action effect, and we can track the rounds used easily enough as well.

- Add a new *Spell Class* for Rage
- Set caster type as *Points(Psion)*
- Set maximum Power Points equal to number of rage rounds per day (4+Con Bonus +2/per level)
- Add a new 1st level *Spell* for Rage 
- Add a *Spell Action* of type *Effect* as laid out in the next section for the Rage condition. 

When you want to Rage, simply click on the effect icon in your Rage spell, and you will automatically gain the effects of Rage. Just click the usage icon each round so that you can keep track of how many rounds have been used. 

#### Core Barbarian
Grants a barbarian +4 Str and +4 Con, a bonus to Will saves and an AC penalty.

*Target*: Self

*Action*: All

*Effect Text*: `Rage;STR:4 morale;CON:4 morale;AC:-2;SAVE: 2 morale will;`

What this **does not** do is automatically add the additional HP granted by the bonus constitution. That will have to remain a manual step - along with removing those bonus HP too!

#### Unchained Barbarian
Grants a barbarian +2 to melee damage and attack rolls, a bonus to Will save and an AC penalty. In addition, the barbarian gains Temporary HP instead of raw HP - this is actually easier to manage in FG than the Core Barbarian!

*Target*: Self

*Action*: All

*Effect Text*: `Rage;ATK:2 melee; DMG:2 melee;AC:-2;SAVE: 2 morale will;`

For Unchained Barbarians, and additional Spell Action should be added in addition to the Rage condition.
- Add a new Spell Action of type Heal
- Set type of healing to *Temp*
- Set value healed to be equal to 2xCL (make sure CL = Barbarian Level when you level up)

When you rage, just use the Healing action on yourself to gain your Temporary HP!



