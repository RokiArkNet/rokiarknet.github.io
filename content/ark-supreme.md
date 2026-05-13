# Ark Supreme — Guide Content

## baseline

All stats based on Level 150 unboosted creatures — no server multipliers or custom imprints. Assumes working knowledge of basic ARK mechanics.

## tier-list

Elite | Savage | Toxic | Berserk | Necrotic | Grenadier | Prime | Nuclear | Vampiric | Wardens | Hellfire | DarkGod | Corrupted Darkgods | Spectral Wardens

## getting-started

You spawn with a 40-second shield — use it to get your bearings and find cover.

Survive long enough to establish a safe location — whether it's a raft base or a small land outpost tucked away from danger.

### Core Crafting Structures

**Supreme Forge** — Smelts metal and alloys.

**Supreme Bench** — Primary station for modded gear, kibble, boss item crafting, potions, and consumables.

**Supreme Bed** — Respawn point.

### The Progression Loop

The first three tiers — Savage, Toxic, and Berserk — follow the same progression loop:

1. **Hunt and harvest** — Kill wild creatures of your target tier and harvest their blood
2. **Craft tranqs** — Use the blood to craft tier-appropriate tranquilizers
3. **Tame** — Knock out and tame creatures of that tier
4. **Establish egg farms** — Breed your tames to produce eggs for the next tier's kibble
5. **Repeat** — Move to the next tier and start again

## cores-essence

Every wild creature drops a tier-appropriate **Dino Core** when killed. **1 Dino Core = 10 Essence.**

- **Cores** are used to craft boss summons.
- **Essence** is an additional ingredient required by all kibble recipes (on top of the eggs the loop already covers).

## elite

Your true entry point. Elite creatures have minor stat boosts above vanilla, making them helpful early-game tames while you prepare to take on Savage tier.

## savage

Your first tiered progression. Hunt Savage creatures for Savage Blood, craft Savage Tranqs, and tame your first Savage dinos. Set up breeding pairs to produce Savage Eggs for Toxic Kibble.

## savage-boss

The Savage Boss is your first boss gate. When defeated, it spawns a tameable version that can be tamed with kibble.

### Savage Snail

The tameable Savage Boss produces **Savage Slime Balls**, which are required for crafting all kibble from Toxic tier onward. Taming this boss is essential for progression.

- Feed berries to produce slime balls
- Can be evolved into a smaller version for easier base storage
- If slime production stops, pod and re-deploy the snail

## toxic

With Toxic Kibble ready, repeat the loop. Harvest Toxic Blood, craft Toxic Tranqs, tame Toxic creatures, and breed them for Berserk Kibble.

Toxic creatures have an AOE ability that inflicts torpor — a powerful alternative to tranqs for knocking out targets.

> During this progression, start growing crops — you'll need them for Berserk Kibble.

## berserk

Same pattern, higher stakes. Berserk creatures hit harder and take more to bring down, but the rewards scale accordingly.

### Berserk Kings

Three Berserk King bosstiers guard entry to Necrotic tier:

- **King of the Swamps** — swamp biomes (sarco variant)
- **King of the Grasslands** — grassland/plains areas (giga variant)
- **King of the Desert** — desert areas (deathworm variant)

You must collect a soul from ALL THREE kings to evolve your Savage Snail into a **Berserk Snail**, which produces Berserk Slime Balls for all kibble from Necrotic tier onward.

> Tame a second Savage Snail before evolving. Kibbles from Necrotic tier onward require BOTH Savage and Berserk slime balls, so you need one of each snail running in parallel. Evolving your only snail leaves you unable to produce Savage slimes.

**Server INIs** (`[ArkSupreme]` section) — cap the number of each King alive in the world at once:

```
MaxKingOfTheDesert=3
MaxKingOfTheGrass=3
MaxKingOfTheSwamp=3
```

## necrotic

Necrotic is where things change. Two new systems unlock here: **Paragon Levels** for cultivating tamed dinos (see [FAQ](#faq)) and **Queen Bee** honey production for higher-tier crafting.

### Honey Production

Wild bees are hostile and attack on sight. To set up honey production:

1. **Kill wild bees** to collect a small amount of honey
2. **Craft Bee Kibble** from that honey at the Supreme Bench
3. **Tame a Queen Bee** with the kibble for sustained honey production

Once tamed, place the tier's rare flowers (crafted at the Supreme Bench) in the bee's inventory — the bee produces honey automatically.

Queen Bees are available across Necrotic, Prime, Nuclear, Vampiric, Hellfire, and DarkGod tiers — each tier's bee uses that tier's rare flowers.

## necrotic-boss

The Necrotic Boss is a **Golem BOSS** that serves as the gate to Grenadier tier.

- **Tameable**: Yes - uses kibble for taming
- **Rewards**: Defeating the boss unlocks Grenadier kibble engrams

## grenadier

Grenadier tier introduces explosive combat mechanics.

### Grenadier Tokens & Factory

Wild **Grenadier Bosses** drop a **Grenadier Token** and a **Grenadier Factory**. To produce **Grenadier Herb** (the key ingredient for Prime Kibble), the factory needs both the Grenadier Token *and* a **Chief Grenadier Token** dropped by the Grenadier Boss Tribesman.

### Grenadier Boss Tribesman

A hostile tribe that can **only be fought with Grenadier-tier or higher tamed dinos**. The chief drops the Chief Grenadier Token required for Grenadier Herb production.

## prime

Prime tier features Guardian bosses that serve as the gate to Nuclear and Vampiric tiers.

### Taming Prime Creatures

To tame Prime tier creatures, you need Prime Kibble made from Grenadier Herb:

1. **Collect Grenadier Herb** — Produced by the Grenadier Factory (see Grenadier section)
2. **Craft kibble** — Use Grenadier Herb at the Supreme Bench to craft **Prime Kibble**
3. **Tame** — Knock out Prime creatures with appropriate tranqs and feed Prime Kibble

### Prime Guardians

Three Guardian bosses exist: Broodmother, Ferox, and Spino. Defeating all three Prime Guardians unlocks Nuclear and Vampiric kibble engrams.

> Prime-tier bosses take reduced damage from anything that isn't a tek-type dino — bring Primes (or higher tek tiers) to fight Primes.

## nuclear-vampiric

Defeating all three Prime Guardians unlocks Nuclear and Vampiric kibble engrams.

## wardens

Only the boss version of Warden creatures spawns in the wild. Killing a wild Warden boss spawns a tameable version on the spot — knock it out and tame it with the appropriate kibble.

This applies to: Warden Rex, Warden Wyvern, Warden Trike, Warden Gorilla, and Warden Manticore.

Wardens are evolved into Spectral Wardens — see the Spectral Wardens section for evolution requirements.

## hellfire

Hellfire creatures use portal-based attacks.

Defeating the Hellfire Boss unlocks DarkGod kibble.

## darkgod

DarkGods are obtained by evolving creatures using a token dropped by the DarkGod King.

### DarkGod Lineup

Available DarkGod variants: Rex, Spider (Broodmother), Crab, Golem, **Griffin**, and **Reaper**.

### DarkGod King

The **DarkGod King** drops the DarkGod token — the key item for evolving DarkGod creatures. The token has a wide pickup radius, so you don't need to land directly on the corpse.

### DarkGod Drops

Defeating wild DarkGods rewards:
- Large XP potions
- Random assortment of Health potions
- Random assortment of Tranqs
- Random assortment of DarkGod-tier Saddles

## corrupted-darkgods

Corrupted DarkGods are the best creatures to use against Spectral Wardens.

### Obtaining Corrupted DarkGods

The Corrupted DarkGod Rex, Broodmother, Golem, **Griffin**, and **Reaper** are obtained **only by evolving their DarkGod counterparts** — they do not spawn in the wild and cannot be tamed directly.

### Corrupted DarkGod King

Defeating the **Corrupted DarkGod King** drops the token used to evolve Wardens into Spectral Wardens.

## spectral-wardens

Spectral Wardens are the final evolution of Wardens.

### Evolution Requirement

Evolving a Warden into a Spectral Warden requires a **Corrupted DarkGod King token**, dropped by the Corrupted DarkGod King (see Corrupted DarkGods).

### Spectral Warden Drops

Defeating wild Spectral Wardens rewards:
- Large XP potions
- Random assortment of Health potions
- Random assortment of Tranqs
- Random assortment of Spectral Warden Saddles

## juggernaut

The Juggernaut is the **final boss** of progression — fought after Spectral Wardens.

### Boss Fight

The Juggernaut now matches Spectral Wardens in strength and is a significant challenge. Defeating it drops a **Tameable Juggernaut Saddle**.

### Tameable Juggernaut

After the Juggernaut boss is defeated, a **Tameable Juggernaut** spawns. Tame it with **Juggernaut Kibble**.

## faq

### Boss Combat

All ground-based bosses will dismount flyers (10 second cooldown) — bring a ground mount for boss fights. Flyer-type bosses (Wyverns, Manticores) are the exception and do not dismount you.

### Tool Harvest Rates

| Tier | Harvest |
|------|---------|
| Savage | 1.5x |
| Toxic | 2x |
| Berserk | 2.5x |
| Necrotic | 3x |
| Prime | 3.5x |
| Hellfire | 4x |

*Hellfire tools have custom materials.*

### Armor Ratings

| Tier | Rating |
|------|--------|
| Savage | 60 |
| Toxic | 100 |
| Berserk | 200 |
| Necrotic | 300 |
| Prime | 400 |
| Hellfire | 600 |

*Per piece. All tiered armor has infinite durability.*

### Tribesman & Lootbosses

Hostile NPCs that spawn in the wild and drop valuable loot when killed. Each Tribesman tier drops items scaled to its own tier.

**Tribesman tiers** (Minion and Chief variants where applicable):
- Savage, Toxic, Berserk, Necrotic, Grenadier, Prime

**Boss Tribesman**:
- **Grenadier Boss Tribesman** — drops the **Chief Grenadier Token** required by the Grenadier Factory to produce Grenadier Herb. Can only be fought with Grenadier-tier or higher tamed dinos.

**Thralls** (higher tiers):
- Prime Thrall with Shotgun
- Nuclear Thrall with Rocket Launcher
- Hellfire Thrall with Flamethrower

**General Drops** — each Tribesman drops a tier-appropriate mix of:
- XP potions (size scales with tier — Tiny → Medium → High → Extra Large)
- Health potions (random assortment, tier-specific)
- Tranqs of their tier and below
- Saddles, Armour, and Tools at their tier
- High-quality weapons from Berserk tier upward (fabricated snipers, longnecks, etc.)
- Ammo and ammo materials (Grenadier Boss Tribesman)
- Taming Cakes (x50, x100, x250) — instantly remove food during taming

**Notable extras**:
- Necrotic Tribesman also drop tameable Necrotic boss saddles
- Prime Tribesman are extremely dangerous — come prepared

### Tribesman Aggression

All Tribesman are now instantly aggressive on sight — no provocation required. When you attack one tribe, nearby Tribesman from neighboring tribes will join in to defend each other. Plan engagements with flanking in mind.

### Paragon Levels

From Necrotic tier upward, your tamed creatures can be **cultivated through 10 Paragon Levels** — a separate progression layered on top of normal taming. Higher levels boost stats and unlock new abilities.

**Level Progression** — Level up by killing wild creatures with your dino. A dedicated UI shows your current Paragon level and progress to the next.

| Level | Reward |
|-------|--------|
| 1–4 | Stat boosts each level |
| 5 | Stat boost + unlocks the **Powerup Ability** (requires defeating a Paragon Boss with that dino) |
| 6–9 | Stat boosts each level |
| 10 | Unlocks the dino's **Supreme version** — major stat upgrade |

**Powerup Ability** — Dinos from Necrotic tier and up are **powered down** at tame time. After completing Paragon level 5 *and* defeating a Paragon Boss with that creature, a button combination unlocks that toggles it between powered-up and powered-down states. Powered-up applies both a visual change and a stat boost.

**Paragon Bosses** — 80 Paragon Bosses can be summoned across the higher tiers. Each summon spawns a random higher-tiered creature with its powerup active — these are the gates required to unlock your dino's powerup at level 5.

Powerups are available on every tier from Necrotic upward: Necrotic, Grenadier, Prime, Nuclear, Vampiric, Wardens, Hellfire, DarkGod, Corrupted DarkGod, and Spectral Wardens.

### Hostile System

Killing Tribesman triggers a **hostile counter** (icon appears in bottom right). As your hostility increases (x2, x4, etc.), more Tribesman will actively hunt you down and their weapons progressively upgrade from spears to longnecks. On servers, hostility persists until cleared. In singleplayer, it times out after 10 seconds.
