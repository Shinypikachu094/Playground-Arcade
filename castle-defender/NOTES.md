# Castle Defender Notes

## How to run

Open `index.html` in a modern web browser. There is no install step and no build step. It also works by opening the file on a phone or by serving this folder with any simple local web server.

## Where it is published

It is currently a local prototype in the Castle Defender project folder. It is not published to the internet yet.

## What is done

- Added rare Blood Moon events that temporarily double horde speed and strength, plus Thunderstorms that can occasionally zap a troop or horseman.
- Added a front shield layer. Shields absorb enemy contact damage one at a time; broken shields leave fallen troops on the road, and Buy Shield replaces a shield troop.
- Wave progress and difficulty now save per territory during play, on refresh, and when a run ends. A new run restores the saved wave/checkpoint difficulty while giving the player a fresh starting squad if the old squad was defeated.
- One responsive survival-runner level with an automatic troop squad, a castle, gates, enemy groups, bosses, checkpoints, and a score.
- Drag or tap left/right on phones. Arrow keys or A/D steer on a computer. Troops fire automatically.
- Game Over and Play Again screens.
- Local leaderboard, troop skin button, and score-based upgrade button.
- All tuning numbers are together in the `CONFIG` object at the top of `index.html`.
- Simple colored shapes are used instead of art.
- Every bullet that hits a gate raises its multiplier by 1: `-2 → -1 → 0 → +1` and so on. The final number changes the squad when the gate is reached.
- Every troop now fires its own bullet in each automatic volley, so bigger squads have more firepower.
- The squad starts smaller and merges every 10 same-tier troops into 1 stronger troop tier.
- Slow enemy mobs now stream continuously with no empty spawn breaks, and the stream stays endless.
- Multiplier gates appear on the left and right sides of each road section.
- Each road section has a breakable boulder on both side edges.
- Side barricades now make a middle corridor for the slow horde. The player can hold the middle and spam shots without losing troops quickly.
- The road is taller for more reaction time, and a mini map shows the squad and incoming horde positions.
- The two multipliers are now at the far-left and far-right edges of the road.
- Checkpoints save the best squad size and restore at least 4 troops instead of dropping the squad to 2.
- The first two multiplier gates are a safe opening; endless hordes begin immediately after the second gate is reached or passes.
- Merging is now optional: press the `Merge Troops` button or the `M` key when the squad has 10 or more troops.
- Troops now show guns and merged tiers add damage power. Enemy health and attack damage increase as checkpoints rise.
- The top-right HUD value is Power; it stays unchanged when only reaching a multiplier or checkpoint and changes from upgrades, merges, or power-ups.
- Troop bodies now stay the same size. Merged troops become armored diamond-shaped units with tier labels and longer gold guns.
- Bullets disappear quickly, and any old bullets are cleared when a merge happens.
- The vertical map is expanded again to give the run more space.
- Mega bosses appear at every fifth checkpoint with much more health and attack damage.
- The squad now has exactly 3 defense rows: front, middle, and back.
- The player can choose each row with the `Front`, `Middle`, and `Back` buttons. The default is giants, gunners, then mages.
- Added squad and enemy health bars. Mages heal the squad and deal splash damage; giants are tanky front-line defenders with reduced incoming damage.
- Rows now have more vertical space. The front row mixes knife guards with giants, stopping normal mobs while bosses can still break through.
- Multipliers are replaced by coins: defeated mobs pay coins, `Buy Troop` recruits troops, and `Build Block` places a defense wall that hordes must destroy.
- Hordes are stronger, faster, and can damage defense blocks while pushing through them. Blocks stop them until destroyed.
- Up to four side crossbows can be bought with coins (two per side). Crossbows auto-fire at enemies, break boulders, collect power-ups, and earn coins from kills.
- Giants were removed. Knife fighters are the stronger front rank, with archers behind them and mages in back.
- Crossbows sit behind the knife fighters. To place a wall, press `Build Block`, then tap or click anywhere on the road.
- Knife fighters now stand farther forward as the first defense line.
- Crossbow ranks now allow three on each side, for six total.
- The squad can move forward/backward with W/S or Up/Down. Build Block enters placement mode, and each tap/click places another block and automatically spends coins until funds run out. Blocks can be upgraded for stronger health and spikes.
- Forward/backward movement now covers almost the whole tall playfield.
- Hordes scale up as checkpoints rise: more health, stronger attacks, stronger archer shots, and more pressure on blocks.
- Horde damage now ramps up much faster: troop hits, archer shots, and block pressure all gain a larger bonus every checkpoint.
- Hordes now have much more health, so normal mobs and archers can tank multiple hits, while their block damage is significantly higher.
- Players can build up to twelve crossbows, unlock the Gunner troop with coins, and choose unlocked troop types for the defensive rows. Hordes now arrive faster and hit harder.
- A thick cobblestone wall starts in the road. Enemies slowly break it, enemy archers can damage it, and the player can repair it with coins. Occasional giant shielded mega leaders chase the squad side-to-side.
- The wall is now heavily reinforced, and six permanent wall guards stand on top and fire at enemy archers and the horde.
- A giant player cannon troop is stationed on the wall and fires a large splash-damage cannonball every five seconds.
- The giant cannon is now the second-row troop in the player squad, with its cannonball fired from the squad formation.
- Horde strength now grows exponentially with checkpoints, including health, troop damage, archer shots, wall damage, and block damage.
- Merging now combines exactly 10 matching-level troops into 1 higher-level troop, allowing mixed squads with many lower-level troops and a few higher-level troops.
- Hordes now spawn across the full road instead of only in the middle lane.
- Boulders show how many hits they need; breaking one releases a power-up that increases troop power.
- Troops grow stronger by tier: every merged tier adds extra damage, so surviving troops can keep earning coins after walls fall.
- The castle now has three layered cobblestone walls. Repair the most damaged layer with the Repair Walls button.
- Players can buy up to three back-line mines. Mines pay coins over time, have health bars, attract enemies, and have stationary guards that shoot attackers.
- Balance pass: regular troops now fire a little faster and hit harder, crossbows are stronger, and enemies move slightly slower so the player can clear normal mobs without making bosses harmless.
- Wall layers now have separate large health pools, mines are much harder to destroy, and enemies that pass the road wrap back to the top with their current health.
- Walls now have much larger health pools, the first 30 seconds are protected so the player can set up, and Repair All Walls restores every wall completely.
- Normal enemies can no longer damage the squad while any wall layer remains; bosses can still break through. The HUD explains that the shared health bar is squad health before troops are removed.
- Every wall now has spikes and a row of flamethrowers that damage enemies pressing it. After all walls fall, new blocks snap into the old wall positions as temporary decoys.
- Added Wall Upgrades: spend coins to increase every wall's max health, spike damage, and flamethrower damage while fully repairing them. Squad upgrades now give a much larger damage boost, and wrapped enemies keep their current health.
- Added an active-enemy limit so the endless horde keeps arriving without filling the whole screen with an unreadable pile-up.
- Fixed gate losses: negative gates now remove actual troop entries, positive gates add actual troops, and Game Over only appears when the real troop list is empty.
- Mines can now be upgraded for coins. Upgrades increase payout, health, and guard damage, and fully repair every active mine.

This update takes inspiration from the broad survival-runner idea of choosing gates and growing a squad, but uses original names, shapes, and code.

## What is next

- Play-test the balance and adjust the `CONFIG` numbers.
- Added a Settings panel with Rose, Violet, and Mint troop skins. The existing Troop Skin button still cycles skins quickly.
- Added Pause/Resume controls and the `P` keyboard shortcut so the player can safely step away without the horde moving.
- Change Skin now pauses the battle and opens a six-skin gallery with distinct shapes, colors, names, and previews. Choose a skin, then return to battle when ready.
- Add nicer art, sound, and a clearer start screen.
- Decide how an online leaderboard should work before publishing.
- Add more troop types and a second level only after Version 1 feels fun.
- Add a clearer gate tutorial and more interesting lane choices.
- Play-test mine placement and layered-wall balance, then add a mine upgrade button if it feels useful.

Balance update: slowed horde health growth and scaled player damage with waves so enemies are no longer effectively indestructible.

Damage fix: wall contact now actively damages hordes, and player damage grows faster while enemy health growth stays gentle.

Wall-stuck fix: wall guards now target enemies already touching walls, and wall contact damage is much stronger.

Wall collision range widened so enemies near the wall are always inside the damage zone.

Mega shield fix: bullets now reduce mega health while also reducing its shield, so shots visibly do damage.

Critical NaN fix: repaired malformed config line breaks so bullet damage uses real numbers again.

Wall balance fix: capped enemy archer arrows at 3% of a wall's maximum health per hit.

Troop placement: added a Place Troop button, up to 60 stationed troops, larger moving rows, and automatic firing for placed troops.

Stationary troop picker added with large previews, pause-while-placing behavior, and a local locker for storing and reusing troop types between matches.

Horde contact fix: enemies now damage the squad at the troop line, remove troops when health runs out, and respawn at the top instead of stopping there.

Wall edge fix: widened all wall layers to cover the road edges and stop bypassing enemies.

Collision fix: wall barriers now cover the entire battlefield width so hordes cannot slip around the visible wall edges.

Graphics pass: added a layered sky gradient, roadside trees, lane highlights, and shadows on the walls.

Added selectable Siege Mode: walls cannot be damaged, enemies pass over them, and archer shots ignore them.

Replaced circle characters with lightweight canvas-drawn human figures for troops, stationed defenders, archers, mages, bosses, and hordes.

Siege Mode correction: hordes now collide with and stop at indestructible walls; archer projectiles still ignore walls.

Bullet range update: extended normal bullet lifetime so shots travel across the full battlefield instead of disappearing mid-screen.

Added territory controls, passive land income, ongoing territory horde pressure, conquest, and purchasable knight compounds with horsemen charges.

Expanded territories to a twelve-region road with wave-gated conquest, quick switching, hidden Gunner unlock, and horse compounds with rapid charges limited to three hits per horseman.

Territory persistence added: switching territories saves the current defense setup and restores each territory's own troops and upgrades.

Made horse compounds placeable buildings, made territory unlocks free with wave gates, extended W movement, and added bullet knockback.

Added farther forward movement and a right-side START-to-CASTLE road progress bar.

Reworked the road map: the progress bar is now nearly full height, W/Up movement permanently records the farthest point reached, and territories unlock by map progress rather than coins or wave number. Horde health and attack power rise as more road is revealed, while mega bosses continue to pressure buildings and troops.

Run loss rule added: after a failed run, the newest conquered territory is rolled back and the next run starts from the previous safe territory so the lost land must be reclaimed.

Coins remain universal across all territories during a run; territory switching only changes that territory's defenses.

Changed the all-territories ending into a long final march: after all 12 lands are owned, the enemy castle stays off-screen and the player must keep holding W/Up to advance through stronger hordes and super bosses.

Added a scrolling road viewport. The screen now represents about 10% of the route, and moving up scrolls the battlefield around the squad.

Extended the final road to five times its earlier length with ten viewport sections. At 90%, the enemy castle appears and switches to rapid horde and boss spawning.

Fixed the short 100% bug by replacing screen-height progress with a real road-distance counter. The player can now keep holding W after reaching the top of a screen.

Fixed the scrolling camera's blue-sky gap by filling the viewport road behind the moving world.

Normal road combat now uses an endless horde stream, so enemies keep arriving ahead of the squad instead of stopping after the first small wave.

Fixed the squad getting stuck at the front edge: once the squad reaches the top of the viewport, holding W scrolls every battlefield object forward so troops and hordes continue through the road.

Centered the advancing squad: while holding W, troops stay near the middle of the screen and the road, walls, buildings, bullets, and hordes scroll around them.

Backward movement added to the same scrolling system: S/Down now moves the squad back along the road and scrolls the battlefield backward too.

Made squad centering follow actual movement instead of keyboard aliases, so forward and backward movement keeps scrolling the road without troops getting stuck.

Territory progression now saves each territory's troops, upgrades, buildings, and road progress. The next territory stays locked until the current one reaches 100%, and the campaign restores after an F5 refresh.

Shortened the pre-castle road from 45,000 to 36,000 distance units so territory completion is easier while keeping the road long.

Added different background themes for all twelve territories, including unique sky, road, edge, stripe, and scenery colors.

Made the front-row knights span the playable width, one-hit normal horde members, and shortened territory roads to 30,000 distance units for easier completion. Bosses remain tougher.

Fixed a soft-lock where an empty defeated squad could be saved and restored by F5 or Play Again. Defeated squads now recover with the starting troops, and the game-over screen reports the correct troop count.

Reduced regular boss health slightly and softened final-road boss scaling while keeping mega bosses stronger.

Added a full-width visible knight line across the playable road so the front defense covers the entire screen.

Changed Play Again so a defeated run restarts in the territory where the player died instead of returning to Home Keep. That territory keeps its saved defenses, while its road progress starts over.

Made territory unlocking use a permanent sequential unlock counter, so West March can only unlock once and the button always advances to the next territory.

Fixed death recovery so Play Again keeps the territory's saved road progress instead of resetting that territory back to 0%.

Horse Compound placement now stays active after each placement and charges the compound cost per click, allowing several compounds to be placed in a row.

Added territory difficulty scaling: enemies gain more health in every later territory, so each map gets harder than the last.

Horsemen now steer toward the nearest living enemy, attack it at close range, and retarget the next enemy after a defeat instead of charging in a straight line.

Reduced lag by refreshing horse targets on a short timer and choosing the nearest enemy with one lightweight scan instead of sorting the whole horde every frame.

Softened territory enemy health scaling from 12% to 6% per territory so later maps are harder without making enemies too difficult to defeat.

Increased horseman charge damage from 25 to 45 while keeping each horseman's three-hit limit.

Added phone support improvements: portrait layout, large tap targets, a fixed no-scroll viewport, and touch rules that prevent accidental zooming during fast taps.

Fixed the land counter so it shows all unlocked territories, even if a territory is temporarily overrun during a run.

Restored vertical scrolling on phones so lower controls are reachable, while keeping horizontal scrolling and accidental zoom disabled.

Unlocked territories are now permanently retained; territory attacks can damage them but cannot remove them from the campaign.
