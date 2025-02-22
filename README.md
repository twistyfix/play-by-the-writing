# Play by the Writing (Play-btw)
### by JeansenVaars

Play by the writing is a small application powered by [Espanso](https://espanso.org/) that enables rolling dice, 
random tables, and playing solo RPG systems directly when writing with your keyboard. Just write down the magic 
keywords (listed below), and they will be replaced with the result of such command, wherever you are typing from.

To put it in plain words, for example, when you write down the command “:qq” (a yes/no oracle), an answer text like
“[No]” or “[Yes, but]” will appear. That’s it!

# Features

- Call your GM emulators right away from your note-taking application:
Mythic 2e, PUM, SUM, GUM, OPSE, MUNE, CRGE, Prompty Questions
- Roll dice anywhere in your system just with a short command,
like `:r2d6+1.` → `2d6+1: 11`
- Seek random tables and roll on them super fast, getting the results in your text
- Use ChatGPT and Dall-E to interact with AI from anywhere (needs OpenAI account) with high levels of customization
- An insane amount of random tables is included to roll right away
- (Advanced) Use nested tables to roll many tables in one go
- (Advanced) Configure your own random tables to access them anywhere

# How to use?

1. Install Espanso (free) before you install Play by the Writing
2. Install Play by the Writing with either the installer, unzipping, or compiling the source code yourself
3. Launch Espanso and play!

For using AI, after installing Play by the Writing, run `:aisetup` - this will ask you for your OpenAI API Key (and place it in $HOME/PlayBTW/config/openai.txt)

Test if everything works by typing `:qq`, if you get an Oracle yes/no answer, you're good to go! Have fun.

[Check YouTube explanation video](https://youtu.be/UeV63Iyi5_s)

## Installable Version

If you are a Windows user, the recommended way to use this is with the installer found [HERE](https://jeansenvaars.itch.io/play-by-the-writing)
There's a price tag on it to justify the work effort overall, for the installer. If you use the open-source version, please consider a donation too.

## Open Source Version

The installable is compilable from the source code available [HERE](https://github.com/saif-ellafi/play-by-the-writing).
If you know some Python and want to fiddle with Espanso, the source code for this is Open Source and Free (consider a donation!)
Instructions included in the source code files.

## Join us on Discord

Would you like to chat about this? [Join us!](https://discord.gg/k2rQMa33Kq)

# What is included?

- **Example kit**: Test before you buy. Once installed, by writing `:example` you should see a happy output.
- **Core kit**: Includes dice rolling, random tables, weighted tables from:
  - [Mythic GM Emulator](https://www.drivethrurpg.com/product/20798/Mythic-Game-Master-Emulator)
  - [Plot Unfolding Machine (PUM)](https://jeansenvaars.itch.io/plot-unfolding-machine)
  - [Scene Unfolding Machine (PUM)](https://jeansenvaars.itch.io/scene-unfolding-machine)
  - [Game Unfolding Machine (GUM)](https://jeansenvaars.itch.io/game-unfolding-machine)
  - [One Page Solo Engine (OPSE)](https://inflatablestudios.itch.io/one-page-solo-engine)
  - [Conjecture Games (CRGE, UNE, BOLD)](https://www.drivethrurpg.com/browse/pub/7251/Conjecture-Games)
  - [The Madey Upy Namey Emulator (MUNE)](https://homebrewery.naturalcrit.com/share/rkmo0t9k4Q)
  - [Storyteller's Prompty Questions (PROMPTY)](https://jeansenvaars.itch.io/storytellers-prompty-questions)
- **AI kit**: Includes Core kit + [OpenAI ChatGPT and Dall-E integration](https://beta.openai.com/playground) 

# What is inside?

- An installer which will setup play by the writing for you
- An executable (Windows, MacOS, Linux) that is run by Espanso to support dice rolling and random tables' logic
- Other configuration files necessary for PlayBTW
- Random Tables as included and used by PlayBTW (plain text)
- Instructions in PDF format (README, INSTALL, KEYWORDS, LICENSE)

# Is this safe?
- Espanso itself is an open-source application
- Play by the Writing is open source, feel free to compile it from source
- Microsoft Windows may consider PlayBTW unsafe, you'll have to trust me, and ignore the warnings or set an exception if necessary
- I am an indie developer; I do most of my stuff for [free and open source](https://github.com/saif-ellafi) - Including Mythic GME Tools for Foundry VTT
- I do this for love. But this took me quite a bunch of hours to get it right. This is why this time I decided to put a minimum price cap for it 😊 Take it as a contribution and a coffee for me

# Executable version instructions

The installer will install everything correctly by default, only change the installer path if you know what you're doing. Just press next until it installs. That's it.

## Installer details

Play by the Writing (Play-btw) files go inside Espanso's user config directory. **IMPORTANT:** Config directory is **NOT** the same as installation directory.

For example, if you install Espanso on the F:/ drive, the **config** directory will still be on the Windows installation drive, where your Documents and user files are located.

The installer will identify this location automatically, so normally you don't have to switch the path installation of Play by the writing.

## Microsoft Windows (10+)

### Installer

1. Make sure Espanso works fine in your system and starts and works correctly (test with `:espanso`).
2. Download the Windows installer executables
3. Follow the installer instructions. By default, the installer should point to Espanso config folder: 
`C:\Users\USERNAME\AppData\Roaming\espanso\`. Adjust if it is different.

## MacOS

1. Make sure Espanso works fine in your system and starts and works correctly (test with `:espanso`)
2. Download the MacOs zip archive
3. Unzip and merge the archive `PlayBTW_v3_01_ai_macos.zip` into `~/Library/Application\ Support/espanso`
You can also run `unzip -o -d ~/Library/Application\ Support/espanso ~/Downloads/PlayBTW_v3_01_ai_macos.zip`

If you accidentally replace, and do not merge and get errors, simply restart the Espanso service and all will be fine.

That's it, test an oracle example with `:qq`.

## Linux

1. Make sure your Espanso installation is valid and espanso starts and works correctly (test with `:espanso`).
2. Download the Zip packages for Linux (either base or base with AI)
3. If using default paths, this should just work: `unzip ~/Downloads/PlayBTW_v3_01_ai_linux.zip -d ~/.config/espanso/`

### AI Complete errors

If you get any errors when using `aicomplete` keyword, it may be due to missing clipboard mechanisms.
Install `xclip` or learn more about it here: https://pyperclip.readthedocs.io/en/latest/index.html#not-implemented-error

That’s it. See the keywords list below in this document.

# Keywords List

The keyword column is what you simply write in your keyboard, to get it replaced with an output (usually, at random).

**Note:** There are some `.` Surrounding certain commands. These represent user input and must be written down to denote the ending.

## Core Keywords

| Name                 | keyword                    | Output                     | Information                                                 |
|----------------------|----------------------------|----------------------------|-------------------------------------------------------------|
| Dice                 | `:dd`                      | 🎲                         | Just fancy dice                                             |
| Arrow character      | `:arr`                     | →                          | Just an arrow                                               |
| Roll dice            | `:r<formula>.`             | 3d6x: [1, 3, 1]            | Complex formulas: https://github.com/borntyping/python-dice |
| Roll fudge dice      | `:df.` or `:df<modifier>.` | ( ) (+) (-) (-) + (3) = -1 | Fudge dice for FATE                                         |
| Roll denesys dice    | `:genesys` or `:gend`      | ...                        | Rolls dice for Genesys RPG by FFG                           |
| Roll Random Table    | `:tt.<tablename>.`         | [Third result]             | Roll from a .txt table based on its filename                |
| Roll Weighted Table  | `:wt.<tablename>.`         | [Next quarter]             | Roll from a .psv table with weights based on its filenam    |
| Update tables        | `:update` or `:pull`       | ...                        | Download and update PlayBTW tables                          |
| Shuffle Poker Deck   | `:shuffle`                 | Shuffled!                  | restarts the poker deck                                     |
| Draw from Poker Deck | `:draw`                    | 8♠ 7♥ 6♦                   | Draws a card from poker deck                                |

## System Keywords (most useful!!!)

| Name                   | keyword   |
|------------------------|-----------|
| BROWSE ALL commands    | ALT+SPACE |
| BROWSE Mythic commands | `:mythic` |
| BROWSE PUM commands    | `:pum`    |
| BROWSE SUM commands    | `:sum`    |
| BROWSE GUM commands    | `:gum`    |
| BROWSE OPSE commands   | `:opse`   |
| BROWSE MUNE commands   | `:mune`   |
| BROWSE CRGE commands   | `:crge`   |
| BROWSE UNE commands    | `:une`    |
| BROWSE BOLD commands   | `:bold`   |
| BROWSE AI commands     | `:aicall` |


## Mythic GM Emulator 2e Keywords

Play with Mythic Game Master Emulator: https://www.drivethrurpg.com/product/422929/Mythic-Game-Master-Emulator-Second-Edition

| Name                                | keyword                                                                                                   |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| BROWSE ALL TABLES                   | `:mythic`                                                                                                 |
| Fate Check (prompted)               | `:mmfc`                                                                                                   |
| Alteration Check (prompted)         | `:mmalt`                                                                                                  |
| Fate Check (per modifier and chaos) | `:mfc<mod>c<chaos>` e.g.: `:mfc+2c4` (+2 modifier, 4 chaos rank) or `mfc-3c9` (-3 modifier, 9 chaos rank) |
| Scene Alteration                    | `:malt<chaos>` e.g.: `:malt6`                                                                             |
| Setup characters list               | `:mlists` or `:mchars`                                                                                                 |
| Roll characters list                | `:mlists` or `:mcharr`                                                                                                 |
| Setup threads list                  | `:mlists` or `:mthreads`                                                                                               |
| Roll threads list                   | `:mlists` or `:mthreadr`                                                                                               |
| Setup adventure features list       | `:mlists` or `:mfeatures`                                                                                              |
| Roll adventure features list        | `:mlists` or `:mfeaturer`                                                                                              |
| Random Event                        | `:mre` or `:mev`                                                                                          |
| Action Question                     | `:mac`                                                                                                    |
| Description Question                | `:mde`                                                                                                    |
| Setup Focus                         | `:mlists` or `:mfocs`                                                                                                  |
| Roll Focus                          | `:mlists` or `:mfocr`                                                                                                  |

## Plot Unfolding Machine v8 Keywords

These are meant to be played with PUM: https://jeansenvaars.itch.io/plot-unfolding-machine

| Name                        | keyword                                            |
|-----------------------------|----------------------------------------------------|
| BROWSE ALL TABLES           | `:pum`                                             |
| Yes or No Deterministic     | `:qq` `:+qq` `:-qq` or with `:qdet`                |
| Yes or No Subjective        | `:qsub` `:+qsub` `:-qsub`                          |
| Yes or No Interaction       | `:qint` `:+qint` `:-qint`                          |
| Random Prompt               | `:scene` or `:prompt` (add +/- for fav/unfav)      |
| Modified proposal           | `:modified` or `:proposal` (add +/- for fav/unfav) |
| Challenge                   | `:challenge` or `:test`                            |
| Catalyst                    | `:catalyst`                                        |
| Complication                | `:complication`                                    |
| Situation                   | `:situation`                                       |
| Focus - What                | `:what` or `:focus`                                |
| Someone - Who               | `:someone` or `:who`                               |
| Intent - Want               | `:intent` or `:want`                               |
| Activity - Doing            | `:activity` or `:doing`                            |
| Place - Where               | `:place` or `:where`                               |
| Reason - Why                | `:reason` or `:why`                                |
| Explain - How               | `:explain` or `:how`                               |
| Time - When                 | `:time` or `:when`                                 |
| Object - What for           | `:object` or `:for`                                |
| Fight - Skills              | `:fight` or `:skill`                               |
| Insight - Notice            | `:insight` or `:notice`                          |
| Discovery - Find            | `:discovery` or `:find`                            |
| Stake - Risk                | `:stake` or `:risk`                                |
| Description - Looks         | `:description` or `:looks`                         |
| How many/much               | `:many` or `:much` (add +/-)                       |
| How good/well               | `:good` or `:well` (add +/-)                       |
| How hard/tough              | `:hard` or `:tough`                                |
| Disruption check            | `:disrupt`                                         |
| Scene starter unblocker     | `:starter` or `:stuck`                             |
| World Elements setup        | `:pnodes` or `:elements` or `:worlds`                           |
| World Elements roll         | `:pnodes` or `:elementr` or `:worldr`                           |
| Meaningful Encounters setup | `:pnodes` or `:encounters`                                      |
| Meaningful Encounters roll  | `:pnodes` or `:encounterr`                                      |
| Things to be Found setup    | `:pnodes` or `:finds` or `:things`                              |
| Things to be Found roll     | `:pnodes` or `:findr` or `:thingr`                              |
| Pending Questions setup     | `:pnodes` or `:pendings`                                       |
| Pending Questions roll      | `:pnodes` or `:pendingr`                                       |

## Scene Unfolding Machine v6 Keywords

These are meant to be played with SUM: https://jeansenvaars.itch.io/scene-unfolding-machine

| Name              | keyword                                     |
|-------------------|---------------------------------------------|
| BROWSE ALL TABLES | `:sum`                                      |
| GM Action         | `:gma` or `:+gma` or `:-gma` (or :gmint)    |
| GM Reaction       | `:gmre` or `:+gmre` or `:-gmre`             |
| GM Factions       | `:gmfac` or `:+gmfac` or `:-gmfac`          |
| PC Matters        | `:pcmatt` or `:+pcmatt` or `:-pcmatt`       |
| PC Backstory      | `:pcback` or `:+pcback` or `:-pcback`       |
| PC Bonding        | `:pcbond` or `:+pcbond` or `:-pcbond`       |
| NPC Attitude      | `:npcatt` or `:+npcatt` or `:-npcatt`       |
| NPC Contribution  | `:npcc` or `:+npcc` or `:-npcc`             |
| NPC Opinion       | `:npco` or `:+npco` or `:-npco`             |
| NPC Impression    | `:npcimp` or `:+npcimp` or `:-npcimp`       |
| NPC Small talk    | `:npctalk` or `:+npctalk` or `:-npctalk`    |
| NPC Truth or dare | `:npctruth` or `:+npctruth` or `:-npctruth` |
| Oracles all       | `:grandoracle`                              |
| Action Prompt     | `:action`                                   |
| Adjective Prompt  | `:adjective`                                |
| Subject Prompt    | `:subject`                                  |

## Game Unfolding Machine v2 Keywords

These are meant to be played with GUM: https://jeansenvaars.itch.io/game-unfolding-machine

| Name                      | keyword                        |
|---------------------------|--------------------------------|
| BROWSE ALL TABLES         | `:gum`                         |
| Exploration               | `:ggexplo`                     |
| Battle location           | `:ggbatt`                      |
| Plot clue type            | `:ggclue`                      |
| Plot useful finding       | `:ggfind`                      |
| Plot enemy activities     | `:ggenemyact`                  |
| Plot recent occurrences   | `:ggoccur`                     |
| Nemesis impression        | `:ggnemesisimp`                |
| Nemesis deeds             | `:ggnemesisdeed`               |
| Nemesis intention         | `:ggnemesisint`                |
| Location by feature       | `:gglocfeat`                   |
| Location by worth         | `:gglocworth`                  |
| Location by purpose       | `:gglocpurp`                   |
| Location by content       | `:ggloccont`                   |
| Character by possessions  | `:ggcharposs`                  |
| Character by intention    | `:ggcharint`                   |
| Character by impression   | `:ggcharimp`                   |
| Character by activity     | `:ggcharact`                   |
| Object by function        | `:ggobjfunc`                   |
| Object by form            | `:ggobjform`                   |
| Object by state           | `:ggobjstate`                  |
| Creature by type          | `:ggcretyp`                    |
| Creature by ability       | `:ggcreab`                     |
| Creature by behavior      | `:ggcrebeh`                    |
| Faction driving focus     | `:ggfacfoc`                    |
| Faction resources         | `:ggfacres`                    |
| Evil motivations          | `:ggmotevil`                   |
| Evil deeds                | `:ggdeedsevil` or `:ggevilact` |
| Good motivations          | `:ggmotgood`                   |
| Good deeds                | `:ggdeedsgood` or `:gggoodact` |
| Grand Oracle (all)        | `:ggorac`                      |
| Grand Oracle (action)     | `:ggact`                       |
| Grand Oracle (adjective)  | `:ggadj`                       |
| Grand Oracle (subject)    | `:ggsub`                       |
| Game setup (location)     | `:ggsetloc`                    |
| Game setup (background)   | `:ggsetback`                   |
| Game setup (mission)      | `:ggsetmission`                |
| Game setup (opposition)   | `:ggsetopp`                    |
| Game setup (motivation)   | `:ggsetmot`                    |
| Game setup (hook)         | `:ggsethook`                   |
| Game setup (initial lead) | `:ggsetlead`                   |
| Game setup (caveat)       | `:ggsetcaveat`                 |
| Game setup (full)         | `:ggsetfull`                   |


## OPSE Keywords

These are meant to be played with https://inflatablestudios.itch.io/one-page-solo-engine

| Name                         | keyword             |
|------------------------------|---------------------|
| BROWSE ALL TABLES            | `:opse`             |
| Oracle (Yes/No)              | `:qa` `:+qa` `:-qa` |
| Set the Scene (Complication) | `:setscene`         |
| Set the Scene (Alteration)   | `:setalt`           |
| GM Moves (Pacing)            | `:pacemove`         |
| GM Moves (Failure)           | `:failmove`         |
| Oracle (How)                 | `:opsehow`          |
| Random Event                 | `:opsere`           |
| Action Focus                 | `:afocus`           |
| Detail Focus                 | `:dfocus`           |
| Topic Focus                  | `:tfocus`           |
| Plot Hook Generator          | `:opsehook`         |
| NPC Generator                | `:opsenpc`          |
| Dungeon Crawler              | `:opsedungeon`      |
| Hex Crawler                  | `:opsehex`          |

## CRGE Keywords

These are meant to be played with https://www.drivethrurpg.com/browse/pub/7251/Conjecture-Games

| Name                        | keyword                                      |
|-----------------------------|----------------------------------------------|
| BROWSE ALL TABLES           | `:crge` or `:une` or `:bold`                 |
| CRGE (Loom of fate)         | `:qkno` or `:qcon` or `:qend`               |
| CRGE Unexpectedly           | `:qunex`                                     |
| UNE NPC Creator Identity    | `:unpc`                                      |
| UNE NPC Creator Motivation  | `:umot`                                      |
| UNE NPC Creator Power       | `:upow` between `:--upow` and `:++upow`      |
| UNE NPC Interaction Mood    | `:umood` between `:---umood` and `:+++umood` |
| UNE NPC Interaction Bearing | `:ubear` others in `:bold`                   |
| UNE NPC Interaction Focus   | `:ufoc`                                      |
| BOLD Waylays                | `:bway`                                      |
| BOLD Connections            | `:bcon`                                      |

## MUNE Keywords

These are meant to be played with https://www.drivethrurpg.com/product/134163/UNE-The-Universal-NPC-Emulator-rev

| Name                     | keyword                   |
|--------------------------|---------------------------|
| BROWSE ALL TABLES        | `:mune`                   |
| Oracle (Yes/No)          | `:mqq` `:+mqq` `:-mqq`    |
| NPC Interaction Attitude | `:matt` `:+matt` `:-matt` |
| Intervention             | `:mint`                   |
| TWENE                    | `:mtwene`                 |

## Prompty Questions Keywords

| Name              | keyword    |
|-------------------|------------|
| BROWSE ALL TABLES | `:question` |
| Any question      | `:prany`   |
| Location          | `:prloc`   |
| Travel            | `:prtrav`   |
| Relations         | `:prrel`   |
| Situational       | `:prsit`   |
| World             | `:prworld` |
| Character         | `:prback`  |
| Faction           | `:prfact`  |
| Crafts            | `:prcraft` |

## AI Keywords (OpenAI)

This experimental functionality relies on OpenAI: https://openai.com for using Artificial Intelligence to autocomplete a prompt. For this to function:
1. Go to openai and create an account (for free)
2. Go to your account settings and copy the API Key
3. With Play by the Writing installed, type `:aisetup` and paste your API Key

| Name                                      | keyword                            | Output                                                       |
|-------------------------------------------|------------------------------------|--------------------------------------------------------------|
| AI OpenAI API Key setup                   | `:aisetup`                         | Setup OpenAI API Key to be used by other commands.           |
| AI ChatGPT New conversation (erases past) | `:aistart`  `:ainew`               | Initialize a new AI ChatGPT interaction. Deletes history.    |
| AI ChatGPT Continue conversation          | `:aichat` `:aiadd` `:aicontinue`   | Continue an initialized ChatGPT conversation                 |
| AI ChatGPT Single question                | `:aiask` `:aisingle` `:aiquestion` | Ask ChatGPT out of the conversation/context (won't remember) |
| AI ChatGPT Show history                   | `:aimemory` `:ailog` `:aihistory`  | Bring AI accumulated knowledge memory                        |
| AI ChatGPT Forget history                 | `:aiforget` `:aierase` `:aiclear`  | Delete AI memories (saves costs)                             |
| AI Image Dall-E 3                         | `:aiimg` `:aiimage` `:dall-e`      | An AI generated image                                        |

# Customization and Advanced usage

## Match files

There are many files with `.yml` extension inside the `match` folder. Open with a text editor and change the lines 
that start with `:` in order to change their command keyword.

Some entries point to `table` (or `wtable` for weighted tables) which follow with a table name. This table name 
is the file name within the folder `tables`, and you can append with comma more than one, i.e. `table1,table2`

Understanding this, will allow you to copy these segments to create your own commands with your own tables!

## Table customization

There are two types of tables. Ones ending in `.txt` (simple tables) and others in `.psv` (weighted tables). Check
the ones available in the folder `tables` for examples of each.

Add your own tables in the `my_tables` folder within the espanso folder to keep your own tables safe and untouched after you upgrade PlayBTW.

You can also copy tables from Espanso's `tables` folder into `my_tables` and change them there, they will be prioritized!

## Nested tables

You can nest table rolls within others, by utilizing the format `{{table_simple_name}}` or `w{{weighted_table_name}}`
where the table name refers to the file name. You can use these however you like, and even build sentences with more
than one of them, i.e. `Hello {{table_1}}, I hope you had a great {{table_2}}!`

# Service Level Agreement of Purchase
- This software is provided as-is, I support users on goodwill and listen to feedback and ideas, but cannot commit to eternal promises.
- This software is only available on itch.io – For your safety, only download from there
- Tested in Windows 11, MacOS Sierra, and Linux (Ubuntu, and OpenSUSE)
- This software is purely and entirely recreational, and it should not cause any harm to your system. I cannot be held responsible for misuse or damage caused to your system.
- Users that have paid, shall receive all future updates for free. However, new content may be sold separately.
- No refunds! Sorry – Use the example package to test this software before you buy

# License - Open Source Code
This application has been made to have fun, and I am not a business. 
You can do whatever you would like to with this software, but be kind, say thanks, and share it with your friends!

JeansenVaars