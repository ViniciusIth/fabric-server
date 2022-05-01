README
Amethyst Imbuement
------------------

Scepters Config:
The scepters config json tweaks the properties of the scepters in-game. You may want to tweak it if you feel like scepters have too many uses at once, or conversely if you feel that they run out of mana too quickly

> opalineDurability: define durability for the Opaline Scepter (Low tier).
> iridescentDurability: define durability for the Iridescent Scepter (mid tier).
> lustrousDurability: define durability for the Lustrous Scepter (high tier).
> baseRegenRateTicks: how quickly the scepters regain mana naturally. Value is in ticks (20 tick per second). 20 ticks is the minimum allowed.


Altars Config:
This json defines functional tweaks for the altars and tables in the mod.

> disenchantLevelCosts: array of the levels required to disenchant the first, second, third, etc. enchantment off a particular item. You can extend this array if you'd like, but it won't do anything unless you also add to the base disenchants allowed. If you allow 3 base enchants, an array up to 7 long would have practical use.
> disenchantBaseDisenchantsAllowed: the base number of disenchants allowed with just the table present before adding pillars. If you want virtually infinite disenchants, make this number very high. You could make it 0, meaning you have to add pillars before you can disenchant at all, but I don't recommend it.
> imbuingTableEnchantingEnabled: disable this to prevent the player from using the imbuing table as an enchanting table. Use this if you have an alternate enchanting system and don't want the table to allow vanilla style enchanting.
> imbuingTableDifficultyModifier: Multiplies the level cost of imbuing by the value entered. A value of 0.5 will halve the imbuing level costs, 2.0 will double them, and so on. Clamped between 0.0 (free) and 10.0
> altarOfExperienceBaseLevels: base number of levels a player can store in an altar of experience surrounded by 0 candles.
> altarOfExperienceCandleLevelsPer: number of storable levels each candle placed around the altar of experience adds. Warding Candles provide double this base bonus.


Colors Config:
This config sets the outline colors for the various ores when seen under the Draconic Vision augment. If an ore is not in these lists, it will appear as the default white outline. Map keys are the ore identifiers, which can be seen with the advanced tooltips turned on (F3+H by default). If an ore is in both a color map and a rainbow list, the rainbow list will take precedence. The mod color map takes precedence over the default one, in case you put a pre-existing color in the mod map, your desired color will still be shown

Precedence: defaultRainbowList = modRainbowList > modColorMap > defaultColorMap

> defaultColorMap: A map of the default colors pre-assigned to vanilla ores.
> defaultRainbowList: List of the vanilla ores that are pre-assigned a rainbow outline
> modColorMap: A map where you can add ores from other mods you are playing with. By default includes some ores from common ore-gen mods
> modRainbowList: List for mod ores you want to appear as a rainbow outline. By default includes some ores from common ore-gen mods


Augments Configs:
These configs allow you to tweak the casting parameters for individual spells. Change these if you perhaps think a spell doesn't cost enough mana, or is too slow between casts

> id: don't change this, or the config will break for that spell.
> cooldown: time in ticks (20 per second) between each cost of the spell.
> manaCost: durability usage of the scepter on each cast. Note the default durabilities in the scepter config to determine proper values.
> minLvl: the minimum scepter level required before the spell can be used in that scepter. Recommend keeping as-is, but may be useful to tweak if you think a spell is too easy to attain, for example.
