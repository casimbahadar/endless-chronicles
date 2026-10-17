# Endless Chronicle

A Fire Emblem style campaign that writes and plays itself in your browser. Every run generates its own world, story, maps and army, then fights its way through five books of war. You can sit back and watch, or take command of your army and play it yourself.

This is a non-commercial fan project. It is not affiliated with Nintendo or Intelligent Systems.

## Playing

Open the site in any modern browser, on a phone or a computer.

To use the original game's art, sound and battle animations, choose your own copy of **Fire Emblem: The Sacred Stones (US)** as a `.gba` file. The game checks the file's checksum (A47246AE) before using it. The ROM is read inside your browser and never leaves your device. No ROM is included with this project.

Without a ROM, choose **Play with simple art** and the game runs with its own simpler graphics.

On a phone you can add the game to your home screen. Once it has loaded fully, it also works offline.

## Controls

- **Watch** lets the army play itself. **Command** lets you give the orders on your turn.
- **Pause**, **Speed** and **New run** control the run. New run asks you to tap twice so it cannot happen by accident.
- **Full map** shows the whole battlefield.
- Tap to move dialogue and cutscenes along.

The tabs below the controls:

- **Army**: your gold, convoy and every unit with their class, weapons and level.
- **Chronicles**: the finished runs, each as a book you can read in the game or download.
- **Fallen**: everyone the army has lost.
- **Options**: settings, including whether story deaths and setbacks happen.
- **Library**: the games the maps and music come from, with how many maps each provides. You can add your own copies of other Fire Emblem games here for more maps and music.

## What a run contains

Each run is five books long. A book is about thirty chapters: a world, a war, a villain and a goal, with the army marching across a world map between battles. A run ends in victory after the fifth book, in defeat when the lord falls, or when you start a new run.

Along the way the generator adds side quests, paralogues (side stories for individual units), ambushes, travel events on the road, a rival with a story of their own, a second army that splits off and returns, recruits who can be talked over from the enemy side, and between books, years of peace in which the army ages and a new generation joins.

Units form bonds through support conversations at four ranks. C, B and A grow a friendship, and at A two units become sworn brothers or sisters, rivals for life, or fall in love. S is for couples only: a proposal, then a wedding chapter where disguised assassins attack the ceremony. Every unit has one of sixteen personalities, which shapes how they talk.

The war has costs. Units can fall in battle, die in story events, be injured, captured or turn traitor, and the people closest to them grieve. These can be turned off in Options.

When a run ends, every unit gets an ending, and the game writes a chronicle of the whole run: each book's war, its notable battles, the cast grouped by generation with their bonds and fates, a memorial and records.

## Hosting your own copy

The site is static, so GitHub Pages or any web host works. Put these files together in one folder:

| File | What it is |
| --- | --- |
| `index.html` | The game |
| `sw.js` | Offline support. Its cache name changes with each release so updates arrive |
| `portraits.js` | Character portraits for cutscenes and the chronicle |
| `community_music.js` | Extra music tracks |
| `csa_more.js` | Extra spell and breath animations, loaded in the background |
| `manifest.webmanifest` | Lets the game install to a home screen |
| `icon-32.png`, `icon-180.png`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` | App icons |

All of them are needed. If one is missing, offline support cannot install.

After uploading a new version, reload the page once or twice so the browser replaces its cached copy.

## Credits

- Fire Emblem and its characters, art and music belong to Nintendo and Intelligent Systems. This project uses them only from a ROM you provide.
- Spell, breath and other battle animations come from the [FE Repo](https://github.com/Klokinator/FE-Repo), made by its community artists, who are credited in the asset folders there (among them SHYUTERz, Arch, Blazer, Norikins, Jubby, HIROTO and Mikey Seregon).
- Extra music comes from the FE-Repo-Music collection (The Unlicense). Runa's songs are used with credit to runa/unuesu.
- Endless Chronicle was designed by Casim and built with Claude.
