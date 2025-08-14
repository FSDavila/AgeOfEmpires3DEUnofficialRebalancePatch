# Age Of Empires 3: DE - Unofficial Rebalance Patch
Download Link for the v1.0 Patch: https://drive.google.com/file/d/1qzRd0nDecN5ox9MFTXAUj33SBJfm8Zv-/view?usp=sharing 
Documentation: https://docs.google.com/document/d/1KgaM2SkVzhgEQrB31pSWVpN9cDU8qg0G2S-pvJZ-SzI
Thread in the AOE3 Forums: https://forums.ageofempires.com/t/age-of-empires-iii-de-unofficial-rebalance-patch/278193

A small but focused Unofficial Rebalance Patch for AoE3:DE, aimed at addressing some long-standing balance concerns — particularly with Ottoman Empire and Baja California (and some outlaws) — while preserving the core feel and flow of the game.

## Why am I doing this?

Certain civs have had a consistent competitive edge in ranked play, leading to exhaustively repetitive matchups (everyone uses Ottoman Empire and Baja California Revolt, and sometimes Brits, France and Spain, leading to the same types of games being played over and over again) and fewer viable strategies beyond spamming what is ‘uber strong’ (or unbalanced) to farm elo.

The official patches were grinded to a halt, with the game being completely abandoned by its developers and managers (in a completely unbalanced state, no less), which prompted me to begin this effort, just like the community previously did in AoE III Legacy with the ESOC Unofficial Patch.

Communication with the official AoE3:DE team has been unproductive, and it’s unlikely we’ll see support for custom ranked queues that permit mods (like this mod or other balance mods in particular) anytime soon. The game still has an active official ranked ladder, and many players will be reluctant to leave it - but that doesn’t mean the community can’t act.
The proposal is to create an Unofficial Rebalance Patch, focused on addressing critical issues such as the Ottomans and Baja California, and of course any other unbalanced mechanic or unit - and invite the community, including top-level players, to help with suggestions for even more precise balancing and adoption.

For championships and normal lobby play, this already works if enough top players and most of the community commit to using it. 

## What about Ranked Ladder?
The main challenge is having a parallel ranked system (there is little to no possibility the DE team would comply if we asked for a Custom Ranked Queue feature), which then requires one of these solutions:

- A custom launcher (similar to W3Champions in Warcraft 3 or the ESOC Patch in AoE3 Legacy). Potentially hijacking the original game’s API calls to point to a custom leaderboard, for games with Data Mods [with this Data Mod in particular] in ranked matches (probably possible through forcing the “Safe for multiplayer” flag for all mods in the game executable) so a leaderboard for a Unofficial Ranked Queue for players using this rebalance mod can actually work properly (both for querying leaderboard/match data to show it in the player UI and to store it to the parallel Ranked Queue server). The same approach is to be used for the actual matchmaking, it is expected to use the elo ratings and metrics retrieved from the parallel leaderboards to do its matchmaking process, all using the original game logic where possible. 

- As a fallback, using the Age3 LAN Server to host matches and record results to an external Ranking Leaderboard maintained by the community (with automated verification of match result via spectator bots joining in all LAN games or even Replay Parsing each replay to determine who won each game and to feed the leaderboard data with elo calculations from this history).

If integration with official ranked matches (or even modding the launcher) isn’t possible, we can still create an external ranking system based on Lobby or LAN matches, with as much automation as possible to keep it simple.

The ultimate goal is simple: take control of the competitive meta away from the official team (which actually has none anyway, as they literally don’t exist) and allow the community to experiment with and maintain its own balance, while keeping the game competitive. The patch is still in testing and many if not all of the current changes to Units, Techs, Cards and other assets, could be reverted or remade in different intensity or direction in its future versions, as more testing and community participation and feedback is done.

## What this patch does (so far):

- Tones down overperforming units and strategies without gutting civ identity (See full changelog below);

- Is compatible with the “Additive Mods” feature from AoE3 DE without any extra intervention. The majority of the changes are simple protomods changes to units done through additive mods that do not alter the files directly;

- Works in all online and off-line matches (normal lobby matches, LAN matches, etc.), except for Ranked queue, which is a separate issue that has to be solved through one  of the above solutions.
If you’re tired of seeing the same civs dominate (to an exhaustive extent) and want to explore a fresher competitive meta, this is your place to be, ^^.

If you have any suggestions about architecture (of the Parallel Ranked Queue solution), unit, tech and card balance tweaking (especially suggestions about the tweaks that are already in the Changelog), or even want to help with coding or other stuff, just send an email to fsdavilagaming@gmail.com, signed with your in-game name.
Let’s make AoE3 ours again, like we did in the good old Legacy times.
— FSDavila Gaming

## Changelog (URP v1.0->Newer Versions):

(Revolution Tech) Baja California:
Max Population increase: Absolute 200 -> +80 Relative (If player has 40 max pop from TC+Houses, Add +80 for a total 120)

(Ottoman Main deck)

The following cards are removed from the Ottoman deck selection:
Mosque Construction
Millet System, Koprulu Viziers, Grand Bazaar, Galata Tower District, Topkapi, Tanzimat, New Order Infantry, and Topçu Corps technologies at the Mosque cost -50%

(Unit) Cuatrero
Big Game Hunting: (automatically activated when attacking with a cooldown of 30 seconds): The Cuatrero lassoes the enemy, temporarily snaring the target and other enemies in an Area of Effect of 2->1 around the target.
HP: 225->210
Damage: 20->19 Ranged
Resistance: 20%->15% Ranged

(Unit) Desperado
Damage: 15->14 Ranged

(Unit) Filibuster
Siege Attack: 25->23 Siege
Ranged Attack: 24->23 Ranged

P.S: The Baja population cap rework will already deal a swift blow against this unit (that already costs 3 pop each), so it is not necessary to nerf it beyond this point.

(Unit) Bandido
Resistance: 25%->20%  Ranged
Damage: 20->18  Ranged
Dynamite Demolition (automatically activated when attacking with a cooldown of 30 seconds): The Bandido throws a dynamite that does 20 damage (50->35 against buildings and ships, 10 against heavy cavalry, 6 against hand shock infantry, and 5 against artillery) with an Area of Effect of 3->2 from a range of 12.

(Unit) Sipahi
HP: 750->700
Hand Attack: 35->32

(Unit) Abus Gun
Ranged attack Damage 36 -> 33 Siege
Range 2-18 
Rate of Fire 3.0 
Bonus damage: 2.50×->2.00x vs.  Light ranged cavalry, 2.50×->2.00x vs.  Ranged shock infantry, 1.75× vs.  Heavy infantry, 0.5× vs.  Artillery , .4× vs.  Cavalry, 0.4× vs.  Shock infantry, 0.3× vs.  Villager

(Unit) Janissary
Cost: 90->100 Food, 25 Coin
Hit Points: 215
Ranged Attack: Damage 20, Range 12, Rate of Fire 3.0
Melee Attack: Damage 15, Rate of Fire 1.5  ×2 vs Cavalry, ×1.5 vs Shock Infantry
Siege Attack: Damage 25 -> 23, Range 6, Rate of Fire 3.0
Other Stats: Resistance 20% Hand, Speed 4.0, Line of Sight 16


(Unit) Great Bombard
Bombard Attack: 500->425 Siege
Resistance: 75%->65% Ranged
HP: 475->450


(Unit) Nizam Fusilier
HP: 210->190
Damage: 20->18 Ranged

Volley Mode: 12 range, 2.0x->1.75x bonus damage against heavy infantry.
Stagger Mode: 12 range, 2.0x->1.75x bonus damage against artillery and siege units.
Melee Mode: 3.0x bonus damage against cavalry and 2.25x against shock infantry.
Defend Mode: 12 range, 2.5x->2.00x bonus damage against cavalry and 1.8x->1.75x against shock infantry.
Stand Ground: 20 range and no bonus damage.

(Unit Type: MercType2 [Spies]) Spies, Muhbirs, Ninjas, Native Scouts, Maigadis, and Inquisitors
Bonus damage Multiplier: 10.00x vs. Outlaw (for Spies and Muhbirs), 5.0x vs. Outlaw (Ninjas and Inquisitors), 2.5x vs. Outlaw (for Native Scouts),  and 1.25x vs. Outlaw (for Maigadis)
