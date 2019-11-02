# MART 391 ST: Game Engines Final Project

## Update for November 1st, 2019:
I'm still on track, if we use the loosest of definitions.  I had allocated 2 weeks to asset creation and we're coming up on that this Tuesday.

Sadly, no code to show for now, but the initial asset files are uploaded to this Git.

### Asset
I finished modeling the tchotchkes that the player will interact with. I need to finish modeling the AI core (10% done), Cannon Frame (40%) (the control station for it is finished), the doors (90%), sleep pod (50%), and the Room itself (30%).  I had to dig into some file format stuff to make sure what I was doing would actually export, but thankfully my preferred modeling software exports most texture channels with their built in FBX Exporter.

Tomorrow and Sunday, I plan to finish off the asset creation phase by finalizing the dialogue script then recording and cleaning up the audio.  I will also be nabbing some sounds from freesound while recording and modulating things as needed.

### Design
I'm not sure if cinematics will be doable at this point, so they are taking a back seat to the rest of the design.

I also think, due to the scales I'm dealing with, the turret mini-game requires a bit of a change.  Fighting the smaller ships will be a bit of a pain, so I think it might make more sense to have them act as static, triggered events in the background while the player's cannon instead focuses on the enemy mothership.  Currently, I still plan to track the squadrons of smaller ships, but instead of fighting them directly, the player will be responsible for power management between charging the main cannon and powering the anti-fighter defenses.  It will be pretty similiar to an auto-clicker game when dealing with the enemy fighters with damage determined by amount of power allocated to the defenses.  However, power is finite so the more devoted to defenses, the slower the cannon can charge and fire at the boss.  The player will also still be responsible for aiming at the boss, but the weapon will now be hitscan.  I feel this will give a more cinematic feel to the game.

### Helpful Stuff
I received an email from Unity about a new FPS Microgame for learning.  I hope to disect the code in it or even incorporate it into my own game to expedite basic things like movement so I can focus on refining the interaction code.
