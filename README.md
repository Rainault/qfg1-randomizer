# General
This program will randomize the location of most items in Quest for Glory 1 EGA. It accomplishes this by generating script/text patch files that the game will load instead of the default resources. As a result, the original game files are not modified, and it's easy to restore the game to its original state.

Only the EGA version is currently supported. (Sorry, VGA fans!) Also, you must be running v1.2 of QFG1EGA. This is the version that you should have if you bought the game on Steam or GOG. Notably, this randomizer will not work on v1.0 (the one called "Hero's Quest").

# Instructions
Windows is the only supported OS at the moment.

Head to https://github.com/Rainault/qfg1-randomizer/releases and download the latest version. Extract the .exe file into your QFG1EGA game folder and run the program from there.

You can provide your own seed if you want (e.g. you're racing against one or more other people, and you all want to be on the same seed), or you can leave the seed empty to have the program generate one for you. Click Patch to generate the patch files.

That's it! You're ready to go on your randomized adventure in Spielburg. If you want to spoil yourself on where everything was randomized to, you can look at the spoiler.txt file.

If you want to restore the game to its original state or generate a new seed, click Unpatch. This will delete the patch files and the spoiler log. You can also do this manually yourself, if you'd prefer -- just delete all SCRIPT.* and TEXT.* files in the game folder.

# Game Changes
Most of the base game rules are left intact, but aside from the fact that items are randomized, the following additional changes should be noted:
* You must complete all three major quests (save Barnard, save Elsa, and banish Baba Yaga) to complete the game. But you are now able to complete them in any order.
  - So, for example, you don't auto-win for leaving Elsa's office without grabbing the mirror (which might not be on her desk!), nor do you auto-win after frogging Baba Yaga. Unless you've already completed the other quests, that is.
* You must have points in both Pick Locks and Magic. Otherwise, you won't be able to access every item location, and thus you won't be able to complete every seed.
* You start the game with no money and no items except for Leather Armor. The Dagger, Lock Pick, and 5 Food Rations are part of the randomized item pool.
  - Starvation is disabled, so you don't need to worry about eating food.
* Shops are also part of the randomization pool, and the prices are randomized. You can "ask about shop" to see what's for sale. Each item can only be purchased once.
* Boris no longer sells the Thief Guild License. The License is part of the randomized item pool.
* Baba Yaga will now give you a randomized item reward for giving her the Mandrake Root.
* You must complete Baba Yaga's Mandrake Root quest before you can turn her into a frog, even if you have the Hand Mirror in your inventory.
* Randomized items that were repeatable in the original game are now one-shot. For example, once you "get mushroom" at the mushroom ring, you can't "get mushroom" again.
* The two Large Brass Key items have been split into separate items. The Kobold's key is called "Glowing Key", and the key to Fred's cave is called "Worn Key".
* You no longer auto-lose for attempting to re-enter the brigand fortress after saving Elsa. This allows you to battle Toro even after you've completed the Elsa quest, or grab items from her desk if you forgot.
* Press Ctrl-K or choose "Loc Check" under "Information" in the menu to view the status of every randomized item location and the status of the three major quests. Unchecked locations are highlighted in blue, and incomplete quests are highlighted in red. Checked locations and completed quests are grayed out.

# Clarifications
These rules aren't any different from the base game, but they deserve clarification in the context of a randomizer.
* With the exception of shops, the command to get a randomized item is the same as in the original game, regardless of what is actually at that location. For example, you should type "get mushroom" at the mushroom ring, even if it doesn't actually give you mushrooms.
* The Flying Falls, Lake Miller (a.k.a. Mirror Lake), and Fairy Dance locations still require an empty flask, even if the dropped item doesn't go into a flask.
  - The Flask of Water and Flask of Fairy Dust items do not require an empty flask at the location where you find them. They will already be in a flask and added to your inventory.
* Beware of combat before you find your Dagger. The game will auto-kill you if you enter combat without a weapon, even if you have some other means of fighting.
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

If you specifically want it to become night, go to the barracks in the castle (west from the courtyard) and "sleep".

## I have all the Dispel Potion ingredients, but the Healer won't accept all of them.
You still need to give the Spirea Seed to the Dryad to learn the Dispel Potion formula.

## How do I enter/exit the Bear Cave if I don't have a Dagger or the Calm spell?
To enter the cave, move to the top of the screen as soon as you enter and wait until the Ogre is close to reaching you. Then loop around the bottom of the screen to get around. Watch this video to see it in action: https://www.youtube.com/watch?v=MWFNCZw58j8&t=75s

When exiting the cave, wait at the cave entrance for a moment, then loop around the same way you came in.

## I found the Dagger, but I can't seem to make additional progress. Do I really have to grind combat?
Probably, but it's not as bad as it sounds. Pick up about 1070 rocks ("get rock" 107 times) to overflow your encumbrance. This will make you very difficult to hit in combat. Then go to the goblin ambush and "fight bush". Dodge repeatedly until you're out of stamina, then escape. Rest, exit, return, and "fight bush" again. Repeat, sleeping at Erana's Peace if necessary. This will get your stats high enough that you should be able to survive difficult fights. Then you just need to grind Weapon Use until you can actually hit the harder monsters.

## What's the deal with "Flask of Miller Lite"?
The game text will describe the two Flasks of Water differently so you know which one you just received, since they're both still called "Flask of Water" in your inventory. "Flask of Miller Lite" indicates that the water came from Mirror Lake, known as Lake Miller in the QFG speedrunning community. It was named after the current world record holder for QFG1EGA any%, misterprmiller.

## I have another question, or I found a bug or have a feature request!
Feel free to create an issue here, or hop onto the QFG Speedrunners Discord (https://discord.gg/ybXNsKJd) and post your question there. We're all a bunch of QFG nerds and would love to have you!
