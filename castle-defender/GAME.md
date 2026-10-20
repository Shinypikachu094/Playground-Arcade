# Castle Defender — Game Plan

## Prototype direction update

The first playable prototype now uses an original survival-runner loop inspired by the broad idea of growing a squad while choosing safer or stronger gates. The player steers the squad left and right, troops fire automatically, and the squad moves toward the castle through enemy groups and checkpoints. It uses original names, shapes, and code.

The current prototype also starts with a smaller squad, merges every 10 same-tier troops into one stronger tier, sends endless enemy hordes, and places boulders on the road. Each boulder needs several bullets to break and then releases a power-up.

## Game idea

**Castle Defender** is a simple game for kids who play games during break. The player is a cannon that shoots friendly troops toward a castle. The troops fight enemies, protect the castle, and can multiply when they touch helpful buffs.

## The player

The player controls the cannon. The cannon is placed on the left side of the screen, and the castle is on the right. Each shot sends out one troop. The player aims by choosing where to shoot.

## Core loop

The player does these things again and again:

1. Click or tap to shoot a troop from the cannon.
2. Help troops move toward and defend the castle.
3. Collect buffs that make troops stronger or multiply them.
4. Stop enemies before they reach the castle.
5. Survive the next wave and try to beat the high score.

## Enemies and obstacles

- **Goblin Runner:** A fast, weak enemy that tries to reach the castle quickly.
- **Stone Brute:** A slow enemy with lots of health that takes several hits.
- **Rock obstacle:** A fixed rock that blocks troops and makes aiming harder.

## Buffs

- **Multiply buff:** Makes one troop become two or three troops.
- **Power buff:** Gives troops extra attack strength for a short time.

## Scoring

The player earns points by defeating enemies. Fast enemies are worth 10 points, and strong enemies are worth 25 points. Collecting a buff gives 5 points. A small bonus is added for surviving each wave. The best score is saved on the leaderboard.

## Win and lose

There is no final win. The goal is to keep going through wave after wave and reach new checkpoints. The player loses when too many enemies get to the castle. After losing, the player can try again and beat the score.

## Controls

The player uses a mouse click on a computer or a tap on a phone. Arrow keys or WASD move the squad left and right; `W`/Up moves it forward and `S`/Down moves it backward. Dragging on the game area also steers it. After a wave ends, the next wave starts automatically after five seconds; pressing **Space** starts it early. Press `P` or tap **Pause** to stop the action when the player needs to leave. Tap **Settings** to choose the troop skin.

## What makes it harder

Every wave gets a little harder. Enemies move faster, appear in larger groups, and stronger enemies show up more often. The player must aim quickly and choose the best time to use buffs.

## Version 1: tiny and fun

Version 1 has **one level** designed to be fun for about 30 seconds. It includes:

1. A short wave-based level with a castle, cannon, troops, enemies, rocks, and buffs.
2. A leaderboard for high scores.
3. A settings screen where the player can change the troop skin.
4. An upgrade area for improving troop power, troop speed, or cannon reload speed.
5. Mouse and touch controls.
6. Checkpoints after successful waves.
7. A paused skin gallery with six distinct troop looks and four separate horde looks, all with previews.
8. A pause and resume button, plus the `P` keyboard shortcut.
9. Designated enemy waves. Finish a wave for coins, then wait five seconds for the next wave or press Space to start it early.

The first version should feel quick, clear, and replayable. The player should understand the game within a few seconds and want to play one more round.

Map expansion: holding W or Up pushes the squad up a long road. The right-side map bar shows the farthest point reached and stays unlocked even if the squad falls back. Territories unlock from road progress, while hordes become stronger as the squad reveals more of the map. Super bosses focus on destroying walls, blocks, mines, and troops so advancing is the goal, not simply reaching the end.

Run loss rule: if a run ends, the most recently conquered territory is lost and the next run starts at the last safe territory. The player must push forward and conquer the lost territory again.

Coins are universal for the whole run. Moving between territories does not move, reset, or split the player's wallet.

After all 12 territories are conquered, the game changes into a long final march. The enemy castle is far beyond the visible screen. The player must keep holding **W** or **Up** to advance, while repeated hordes and super bosses get stronger and attack the player's buildings and troops.

Road camera: the screen is a small viewport showing about 10% of the road. Moving upward scrolls the battlefield so new road appears above the squad instead of showing the whole journey at once.

Final road: after all territories are owned, the road is five times longer than before and is divided into ten viewport sections. The player keeps holding W/Up to advance through sections 1–10. At 90%, the enemy castle appears and rapidly sends hordes and bosses.

The road percentage now uses a real long-distance counter. Reaching the top of one screen no longer completes the road; holding W continues adding distance across the full route.

Balance update: Horde health now grows gently, boss shields are lower, and player weapons gain damage as waves advance so the horde stays challenging but beatable.

Troop placement update: players can station troops anywhere on the battlefield. Stationed troops leave the moving squad, act like defensive buildings, and fire automatically.

Stationary troop picker: players can choose a Knife Fighter, Archer, Mage, or Cannon with a large preview. Choosing and placing pauses the battle. Troop types can be stored locally for later matches.

Horde contact update: when a horde touches the squad line, it damages and can remove troops, then returns to the starting line with its remaining health.

Wall edge fix: each wall now covers the full playable road so enemies cannot walk around the right or left side.

Second mode: Siege Mode makes walls unbreakable. Hordes and archer shots pass over them, so players defend with troops, blocks, mines, and other defenses.

Character graphics update: troops and hordes now use original human-style figures with heads, bodies, arms, legs, weapons, and role-specific colors.

Siege Mode wall rule: hordes are blocked by the unbreakable walls, while archer shots still pass over them.

Territory expansion: players can conquer West March, North Reach, and East Vale. Owned territories generate coins and face ongoing horde pressure, while knight compounds send horsemen charges.

Long road update: the map now has twelve territories leading to the Enemy Castle. New land unlocks one territory at a time after the current road reaches 100%, and left/right buttons quickly switch between owned territories. Gunner unlock was removed.

Territory defenses are now separate: troops, walls, blocks, mines, crossbows, power, horse compounds, and upgrades stay in their territory when the player moves.

Movement and combat update: hold W to push farther up the road, territory unlocks require reaching 100% rather than coins, and friendly bullets knock hordes backward.

Territory progression: each territory must reach 100% before the next territory can be unlocked. Each territory keeps its own road progress, troops, walls, buildings, and upgrades when switching. The campaign save also survives a browser refresh with F5.

The pre-castle road is tuned shorter so reaching 100% is achievable without making the territory feel tiny.

Knight balance: front-row knights spread across the whole playable road and defeat a normal horde member in one hit. Bosses and mega bosses still need repeated attacks.

Map backgrounds: each territory has its own color theme and scenery colors, so changing territories is easy to notice.

Territory difficulty: enemy health increases with every territory, making each new map harder than the previous one.

Road progress update: holding W or Up moves farther toward the castle, and a vertical progress bar on the right shows the squad's road position.
