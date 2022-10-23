# General
This program will randomize the location of most items in Quest for Glory 1 EGA. It accomplishes this by generating script/text patch files that the game will load instead of the default resources. As a result, the original game files are not modified, and it's easy to restore the game to its original state.

Only the EGA version is currently supported. (Sorry, VGA fans!) Also, you must be running v1.2 of QFG1EGA. This is the version that you should have if you bought the game on Steam or GOG. Notably, this randomizer will not work on v1.0 (the one called "Hero's Quest").

If you have questions, find a bug, or just want to chat with a bunch of fellow QFG nerds, join the [QFG Speedrunners Discord](https://discord.gg/QwhuWWH). We'd love to have you!

And if you enjoy the randomizer and would like to buy me a metaphorical coffee to say thanks, you can do so [here](https://ko-fi.com/rainault).

# Antivirus/Malware Note
I've received reports that some antivirus/malware programs are reporting the randomizer application as a trojan. (I guess modding a game by dumping a bunch of extra files into a folder does look suspiciously like a trojan.) I am currently working on resolving this problem in a more permanent fashion, but you may need to tell your antivirus/malware program to allow the randomizer to run. Sorry for the inconvenience!

# Visual C++ Redistributable
If you get an error message that says "The application was unable to start correctly (0xc000007b)." when attempting to launch the randomizer, you are missing the Visual C++ Redistributable, which is required to run the randomizer. You can download and install it from [here](https://aka.ms/vs/17/release/vc_redist.x86.exe). I will be attempting to remove this dependency in the future.

# Instructions
Windows is the only supported OS at the moment.

Head to https://github.com/Rainault/qfg1-randomizer/releases and download the latest version. Extract the .exe file into your QFG1EGA game folder and run the program from there.

The interface should (hopefully) be pretty self-explanatory -- set the options you want, and click "Randomize" to generate a new patch. The customization options all have tooltips to explain what they do.

There is also a new Help tab that answers questions you may have about how different aspects of the randomizer works, so please do check that out.

If you are trying to have a group of people play the same seed, you can generate your own randomization, "Copy" the seed/flags string (which should look something like this: "2504080195:C3A1Mf"), then give this string to everyone else and have them click "Manual Seed" to generate the same shuffle that you generated.

If you want to spoil yourself on where everything was randomized to, you can look at the spoiler.txt file. The file also includes EgoBot's path through the game to ensure that the generated seed is beatable.

If you want to restore the game to its original state or generate a new seed, click "Clean". This will delete the patch files and the spoiler log. You can also do this manually yourself, if you'd prefer -- just delete all SCRIPT.* and TEXT.* files and the spoiler.txt file from the game folder.

# All 60 randomized item locations
* Bird nest in front of Healer's Hut
* Henry's cave
* Meeps (2x)
* Mushroom ring (2x)
* Spirea plants
* Erana's Peace (2x)
  * Erana's stone excluded for heroes without Magic
* Flying Falls
* Lake Miller
* Sam's reward
* Abdulla's reward
* Wolfgang's reward
* Healer's reward
* Fox's reward
* Brauggi's reward
* Dryad's reward
* Visit Erasmus
* Beat Erasmus at Mage's Maze
  * Excluded for heroes without Magic
* Graveyard
* Old lady's house (5x)
  * Excluded for heroes without Pick Locks
* Sheriff's house (5x)
  * Excluded for heroes without Pick Locks
* Survive the Dragon's Breath
* Beat the Chief at Dag-Nab-It with a bet of at least 25 Silver
  * Excluded for heroes without Throwing or both Stealth and Pick Locks
* Ogre chest
* Kobold cave (3x)
* Beat the Weapon Master
  * Excluded for heroes without Parry
* Baron's reward
* Brutus's body
* Garbage pile in Fred's lair
* Fred's beard
* Toro's body
* Elsa's office (2x)
* Baba Yaga's reward
* Cheetaur's claws
* Troll's beard
* Zara's magic shop (3x)
* Dry goods store (4x)
* Hilde's stall (2x)
* Healer's shop (1x)
* Thieves' Guild (2x)
  * Excluded for heroes without Stealth and Pick Locks
