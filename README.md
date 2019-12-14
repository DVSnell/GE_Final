# MART 391 ST: Game Engines Final Project

## Finals Update, December 13, 2019:
###
Added interaction and audio capability.  This ended up being a bit tricky as Unity's audio systems are about as clear as mud, but I got something functional out of it.  Unfortunately, I wasn't able to implement the Turret game, but I did get a basic start screen set up.

Design docs, testing results, and final game uploaded to Git.

[Timeline and presentation](https://docs.google.com/presentation/d/1yK1uODOAqhezgVXdhOKphzRICeuSqtxCaMDtMA3p-is/edit?usp=sharing)

Trailer located at:
https://youtu.be/iemtGXk-bBI

Personal notes:  I learned a ton doing this.  I was also able to use this project for my Producing class to generate a prospective budget and timeline.  It was enlightening, especially when compared to other Indie project budgets.  I think this is an idea I will continue to refine as time goes on and I pick up more skills.

## Update for November 15th, 2019:
### Update on implementation details.
Rough Assets are done.  Player has movement control.  I'm basing a lot of the implementation on the FPS Microgame from the Asset Store.  The level is laid out with fixed assets.  Interactable objects are not implemented yet, nor is the interaction function, but I'm looking at repurposing the Microgame's look-down-sights function to act as our inspector/event trigger.

### Please indicate who has worked on what part of the project.
I mean... me.  It's just me.

### Specify how your timeline has changed.  Include your old timeline and your new timeline if changed.  Be as specific as you can be with your timeline.
Here is my original timeline:
- Asset Creation - 2 weeks (Continual Refinement)

     Models and Audio
     Unity Materials/Shader Scripting
- Movement and Interaction Scripting  - 2 weeks
- Turret Sub-Game - 2 weeks

     Health mechanisms
- Trailer/Marketing - 1 week

     Design Finalization
- Testing - Entire Duration with focus in last 2 weeks.

I'm currently at the 2nd Week of Movement and Interaction Scripting.  I admit that I'm a little behind and only really getting started with the interaction side of things.  I also skipped working on the shader side of things for now since I decided it was more important to focus on function over style for now.  Style is something I can iterate over in the future.  I am also looking a bit ahead at the turret game and thinking of how to solve things I don't know yet like switching camera's, clamping rotation in the controller and toggling control options based on game states.

### Include achievement components, social components, and immersion components of your game.
The desire to move the game forward and explore more of the setting's background by listening to more audio events from interacting with the objects.  It is continued with the turret game by allowing the providing the player with actual win/lose states.  There aren't a lot of social apart from sharing information after-the-fact or competitiveness in the form of speed-running.  Immersion is a bit trickier since there is no character customization and I am intentionally avoiding gendered pronouns in reference to the player.  I hope to sell immersion through the world and, eventually, with improved visuals.

### Discuss the skills required in your game
The skill bar is fairly low.  Understanding of basic controls and ability to follow prompts are all that is required.  Some sense of timing will be required in the final turret level where the player faces off with the boss ship.  At it's core, basic cognition is the only real requirement.

### What the goals are of the game (how will the players know what the goals are)
The goal is to reach the end.  There are only two (three if we count quitting early) possible times this can not occur, both inside the turret game.  The player will be provided prompts by the AI character which act as both tutorial and guidance.

### What is the constant feedback that your game provides to the players
Visual feed back is primary since it is a video game, but there will also be auditory components like footsteps, ship sounds, and AI dialogue.

### How does your game make players less self-absorbed?
The concept of the game is fighting for your home and inspecting objects left by previous occupants of the room which I hope the player would think back upon later.


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
