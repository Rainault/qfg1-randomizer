# General
This program will randomize the location of most items in Quest for Glory 1 EGA. It accomplishes this by generating script/text patch files that the game will load instead of the default resources. As a result, the original game files are not modified, and it's easy to restore the game to its original state.

Only the EGA version is currently supported. (Sorry, VGA fans!) Also, you must be running v1.2 of QFG1EGA. This is the version that you should have if you bought the game on Steam or GOG. Notably, this randomizer will not work on v1.0 (the one called "Hero's Quest").

# Antivirus/Malware Note
I've received reports that some antivirus/malware programs are reporting the randomizer application as a trojan. (I guess modding a game by dumping a bunch of extra files into a folder does look suspiciously like a trojan.) I am currently working on resolving this problem in a more permanent fashion, but you may need to tell your antivirus/malware program to allow the randomizer to run. Sorry for the inconvenience!

# Instructions
Windows is the only supported OS at the moment.

Head to https://github.com/Rainault/qfg1-randomizer/releases and download the latest version. Extract the .exe file into your QFG1EGA game folder and run the program from there.

There are several customization options to choose from to tailor your randomization experience; the tooltips should explain what each one does.

You will also need to assign a class to your hero now, as well as decide which skills you want your hero to have. This allows the randomizer logic to take into account which locations you can access using your skills. For more randomizer fun, you can also choose to be Classless. In addition to randomizing your initial attribute values, it will also randomly select which of the six skills (Parry, Stealth, Pick Locks, Throwing, Climbing, Magic) your hero will have access to. You can guarantee access to any of those skills if you prefer.

If you are trying to recreate a certain seed (e.g. you're racing against one or more other people), you can copy the seed/flags string, which should look something like this: "2504080195:SHPLr". Pasting this into the randomizer will also recreate the selected customization options, since they are necessary to ensure that the randomizer produces the exact same results.

Once you're ready, click Patch to generate the patch files. Now you're ready to go on your randomized adventure in Spielburg. If you want to spoil yourself on where everything was randomized to, you can look at the spoiler.txt file.

If you want to restore the game to its original state or generate a new seed, click Unpatch. This will delete the patch files and the spoiler log. You can also do this manually yourself, if you'd prefer -- just delete all SCRIPT.* and TEXT.* files in the game folder.

# Game Changes
Most of the base game rules are left intact, but aside from the fact that items are randomized, the following additional changes should be noted:
* You must complete all three major quests (save Barnard, save Elsa, and banish Baba Yaga) to complete the game. But you are now able to complete them in any order.
  - So, for example, you don't auto-win for leaving Elsa's office without grabbing the mirror (which might not be on her desk!), nor do you auto-win after frogging Baba Yaga. Unless you've already completed the other quests, that is.
* You start the game with no money and no items except for Leather Armor. If "survival mode" is ON, you also start without your weapon. Fighters get to keep their Shield.
  - Starvation is disabled, so you don't need to worry about eating food.
* Press Ctrl-K or choose "Loc Check" under "Information" in the menu to view the status of every randomized item location and the status of the three major quests. Checked locations and completed quests are grayed out.
* Shops are also part of the randomization pool, and the prices are randomized. You can "ask about shop" to see what's for sale. Each item can only be purchased once.
* Boris no longer sells the Thief Guild License. The License is part of the randomized item pool.
* Baba Yaga will now give you a randomized item reward for giving her the Mandrake Root.
* You must complete Baba Yaga's Mandrake Root quest before you can turn her into a frog, even if you have the Hand Mirror in your inventory.
* Randomized items that were repeatable in the original game are now one-shot. For example, once you "get mushroom" at the mushroom ring, you can't "get mushroom" again.
* The two Large Brass Key items have been split into separate items. The Kobold's key is called "Glowing Key", and the key to Fred's cave is called "Worn Key".
* You no longer auto-lose for attempting to re-enter the brigand fortress after saving Elsa. This allows you to battle Toro even after you've completed the Elsa quest, or grab items from her desk if you forgot.

# Clarifications
These rules aren't any different from the base game, but they deserve clarification in the context of a randomizer.
* With the exception of shops, the command to get a randomized item is the same as in the original game, regardless of what is actually at that location. For example, you should type "get mushroom" at the mushroom ring, even if it doesn't actually give you mushrooms.
* The Flying Falls, Lake Miller (a.k.a. Mirror Lake), and Fairy Dance locations still require an empty flask, even if the dropped item doesn't go into a flask.
  - The Flask of Water and Flask of Fairy Dust items do not require an empty flask at the location where you find them. They will already be in a flask and added to your inventory.
* If a hero without Magic finds or purchases a spell scroll, only a Piece of Paper will enter their inventory. They will not learn the spell.
* The Healer still sells Healing/Vigor/Mana Potions at the normal prices. The Undead Unguent slot is randomized, however.
* The Healer accepts the same components and gives the same compensation for them as the base game.
* You still need a Thief Guild License to deal with Boris, including asking him what he is selling.
* Boris accepts the same stolen goods and pays out the same rate for them.
* Quests require the same items -- e.g. the Gold Ring goes to the Healer. But what they give you will probably be different.
* The Dispel Potion formula is unchanged, and the Healer will still give you the Dispel Potion for those ingredients.

# All 52 randomized item locations
* Bird nest in front of Healer's Hut
* Henry's cave
* Meeps (2x)
* Mushroom ring (2x)
* Spirea plants
* Erana's Peace (2x)
* Flying Falls
* Lake Miller
* Healer's reward
* Brauggi's reward
* Dryad's reward
* Graveyard
* Old lady's house (5x)
* Sheriff's house (5x)
* Ogre chest
* Kobold cave (3x)
* Baron's reward
* Brutus's body
* Garbage pile in Fred's lair
* Fred's beard
* Toro's body
* Elsa's office (2x)
* Baba Yaga's reward
* Cheetaur's claws
* Troll's beard
* Beating Erasmus at Mage's Maze
* Zara's magic shop (3x)
* Dry goods store (4x)
* Hilde's stall (2x)
* Healer's shop (1x)
* Thieves' Guild (2x)

# FAQ
## I need to make time pass by. What's the fastest way to do so?
Go to the tavern, walk up to Crusher, and "ask about guild". This will advance time forward by one step (and may kill you if you only have a couple HP left).

If you specifically want it to become night, go to the barracks in the castle (west from the courtyard) and "sleep". Note that this won't work if "sunset approaches".

## I have all the Dispel Potion ingredients, but the Healer won't accept all of them.
You still need to give the Spirea Seed to the Dryad to learn the Dispel Potion formula.

## How do I juke the Ogre?
When you enter the Ogre room, move to the top of the screen and wait until the Ogre is close to reaching you. Then loop around the bottom of the screen to get around. Watch this video to see it in action: https://www.youtube.com/watch?v=MWFNCZw58j8&t=75s

When exiting the cave, wait at the cave entrance for a moment, then loop around the same way you came in.

## How do I kill the Kobold using Flame Dart when I don't know Dazzle?
You gotta be fast. It helps to slow down the speed a bit. Each Flame Dart has to come out as soon as you regain input after casting the previous one. If you're too slow, the Kobold will cast Reversal, and your Flame Darts will become useless.

## How do I get the Kobold's mushrooms and chest while the Kobold is alert?
Dazzle is the easiest way to do this, but otherwise, you gotta be fast and a bit lucky. Healing potions help. If you keep dying, try grinding your max HP up so you can survive a couple bolts.

## How do I get the Mandrake Root without Undead Unguent?
Enter the graveyard from the north, "get root" as soon as you are in the graveyard, then run due south. You can also backtrack north, but the movement is a bit trickier and harder to manage before the ghosts get you.

## How do I avoid Toro without sneaking?
If you know the Open spell, cast it while hiding in the bushes. Then wait until Toro is about at the midpoint of the screen, and make a beeline for the gate. You should have barely enough time to "open" the gate and get inside before Toro notices you.

If you don't know Open, you'll have to reach the spot behind the boulder on the top-right of the screen to climb up the gate. The timing for this is *very* tight, so you'll probably need to practice this a bunch.

## I found the Dagger, but I can't seem to make additional progress. Do I really have to grind combat?
Probably, but it's not as bad as it sounds. Pick up about 1070 rocks ("get rock" 107 times) to overflow your encumbrance. Make sure you can still move around without being encumbered -- if you still move slowly, you need to pick up more rocks.

Overflowing your encumbrance will make you very difficult (but not impossible) to hit in combat. You'll still need to grind your stats high enough to actually defeat any monsters, but this should make it a lot more feasible.

## Help! I need more money!
Don't forget you can sell Mushrooms to the Healer. If you have the Toadstools, you can drop all of them on the ground and pick them back up again, and the game will forget that they were Toadstools.

Once you have the Thief Guild License, you can sell the Alabaster Vase, Music Box, Silver Candlesticks, Candelabra, and String of Pearls to Boris. (You can also sell the Glowing Gem and Gold Ring, but I'd advise against that.)

If you have the Dagger, you can grind brigands or trolls east of Fred's cave.

Barring all that, you can work at the stables for 5 Silver. It's a slow grind, but you shouldn't be required to do it unless you squandered your money, you turned off the "fair shop prices" option, or there's a bug that I need to fix.

## What's the deal with "Flask of Miller Lite"?
The game text will describe the two Flasks of Water differently so you know which one you just received, since they're both still called "Flask of Water" in your inventory. "Flask of Miller Lite" indicates that the water came from Mirror Lake, known as Lake Miller in the QFG speedrunning community. It was named after the current world record holder for QFG1EGA any%, misterprmiller.

## I have another question, or I found a bug or have a feature request!
Feel free to create an issue here, or hop onto the QFG Speedrunners Discord (https://discord.gg/ybXNsKJd) and post your question there. We're all a bunch of QFG nerds and would love to have you!
