Noted Irregularities

- Enemies using Player's PSPD for homing projectile aiming
- DONE Drones not disappearing when Player dies
- Barrage projectiles not inheriting Bounce or other attack properties
- Rampage not providing additional effects after a point
- "Increases/decreases in X added as Y" does not isolate the increase/decrease, preventing counterbalancing
- "200% increased Cycle Speed while Boosting" using same effect as Swapper buff
  * Means Swapper and this effect don't stack
  * Means Swapper buff ending force-removes this effect
- DONE Holding down Boost to automatically consume Boost does not trigger effects for when Boost starts
  * DONE "100% Increased Luck While Boosting" repeatedly halves Luck PERMANENTLY due to this
  * DONE "Launch Homing Projectile While Boosting" gets disabled due to this
  * DONE "Increased Cycle Speed While Boosting" gets disabled due to this
  * DONE "Invulnerability While Boosting" gets disabled due to this
- DONE Releasing the Boost key triggers on-Boost-end effects even if the player wasn't actually Boosting
  * DONE Once again triggers "100% Increased Luck While Boosting" halving Luck PERMANENTLY
  * DONE If you run out of Boost while holding down the button for any reason, you're screwed
- "100% Increased Luck While Boosting" is actually "100% More Luck While Boosting"
- Duplicate Stat Boosts don't refresh each other
  * Old Stat Boost timer sticks around and forces the Stat Boost to end early
- DONE Attack Pickups inherit the font size of the pause/score screen


Extra Projects

- Code refactoring
- Optimize projectile trails (!!!)
- Optimize explosion particles (!!!)
- Optimize projectile death particles (?)
- Optimize projectiles
- Change Attack/Resource bar colors to match any forced behavior
- Add indicator for remaining Item spawns
- Change/Remove Projectile Cap (after optimizations)
- Adjust projectile trail size to match projectile size
- Redesign the Stat system to be more consistent and reliable
- Add a stat overview when hovering over the central tree node
- Allow respeccing classes directly in the Classes menu
- DONE Add a hotkey to enable debug mode
- Show actual stats in the device menu instead of being vague


Rebalancing Possibilities

- Make Shield Projectiles hereditary, and only from weapon fire
  * Current behavior makes non-Shield explosions and splits also create shield proejctiles, which isn't fun
- Move Random Attack from Items to the Attack pool (as a ? drop)
  * Random Attack feels like a waste, rather than a help, and defeats the purpose of Items
- Remove Classes, duplicate keywords, and build-breaking results from the Item pool
  * Results like these make Items both too powerful and too negative at times
- Remove/reduce Enemy Health Scaling, reimplement Enemy Spawn Scaling, implement Enemy Damage Scaling
- Make "Invulnerable While Boosting" also cause Boost cost to increase with time
  * It was possible to make a completely immortal build because it never ran out of Boost
- Ability for Bouncer class: Allow Bounce projectiles to bounce off of enemies for extra damage (?)
- Allow Drones to Attack Twice (?)
- Replace On Item Pickup nodes with On Attack Pickup (?)
  * Items are a scarce and limited resource, making these underperform
  * Would increase the value of Only Spawn Attack as a viable option
- Redesign Rampage to lose stacks consecutively, but decrease stack duration the more you have
  * Meant to prevent situations where you have so much Rampage your projs phase through enemies
  * Unsure what to do with the threshold bonus effects