# nst_ap_tool
Crash Bandicoot N.Sane Trilogy Archipelago Mod and Save Editor

Before I get into anything: AI disclaimer. This tool has been created by AI. The research and implementation were AI assisted. The testing and refining in each step was done by me. I am not a developer, I know a few ways around python, this has been a deep dive into the world of memory, reverse engineering and lots of interesting things I learned about the game. I understand that these days people hate to see AI usage anywhere and anytime, but this isn't the place for opinions or discussions about it. I have started this as a passion project for myself, and I am sharing this as a working client (at least on my end, running Fedora Linux) for people to play this game with some randomized elements. I am planning to add and change more, just wanted you to know that I do this with my heart, not prompting "AI please reverse engineer and add this and that into the client". As of writing this, I have started the project about a month ago.

That said, if you're a Software developer and would like to create a non AI version of the client or just contribute, feel very much free to do so and to contact me for any questions I could answer in regards to it. I would also like to take this opportunity to thank the Crash and Skylanders Community and the amazing people who do modding for those games aswell.
Big shout out to the Skylanders Reverse Engineering Discord, the guys and gals in there helped me solve one of the biggest riddles I encountered while working on the AP and understanding the save file, with which the whole adventure started. Lots of love!

I guess I am lazy but it's also late, I've checked the manual the agent created and added some disclaimers or additional information where I deemed necessary.




**Archipelago multiworld support for Crash Bandicoot N. Sane Trilogy** — all three games in one
run. Gems, crystals, relics, keys, bosses and level completions are checks; gems, crystals,
relics, keys and Crash 3 power-ups are items.

The tool runs next to the game: it detects your checks, talks to the Archipelago server, and
writes received items into the running game. No game files are modified.

- **PC (Steam):** Windows, or Linux through Proton
- **PS4 version:** through shadPS4 on Linux

Also included: a save editor, a live monitor, and an optional in-game notification overlay.

## Quick start

1. Install **Python 3.10+** (with tkinter) and **Archipelago 0.6.0+**.
2. In this folder: `pip install -r requirements.txt`
3. Start: `python3 main.py` (Windows: `py main.py`)
4. *Save editor → Install AP baselines…* (your saves are backed up first)
5. *AP Options*: set up your run → *Archipelago → New local game*, or *Connect* to a server
6. Start the game and press **Continue**

On Linux, the tool needs permission to access the game's memory — see the manual.

**Hosting a multiworld?** Players create their YAML in the tool (*AP Options → Save YAML…*);
the host needs **`crash_nst.apworld`**, included in this release.

📖 **Everything else — installation details, what happens to your saves, multiplayer, known
limitations — is in [MANUAL.md](MANUAL.md).**

## Status and plans

Version 1.0 Beta. 
Planned: level shuffles, extra AP crates in levels, in-game item text, and
CTR: Nitro-Fueled support (in research).

**Found a bug, or something that doesn't work at all? Please open an issue** — see the manual
for what to include.
