# Friday Night Funkin' - Stellar Engine
totally not another psych fork!!!!! you cant believe me, right?

i give up

## Installation:

You must have [Haxe](https://haxe.org/download/), installed in order to move on to these next steps

---

Go into your `setup` folder located in the root directory of the source code, and execute the respective script for your operating system

`setup-unix.sh` was designed for Linux and Mac, `setup-windows.bat` was designed for (duh) Windows

for Windows users, double click the `setup-windows.bat` file, and wait until the process of installing the libraries is finished

---

for Linux and Mac users, often double clicking on `setup-unix.sh` is the solution, but if not, open up a terminal on the script's folder location, and execute the following command:

`sh setup-unix.sh`

---

once finished, you should be ready to compile, you can open a terminal in the source code folder, and then type `lime test <target>`

with `<target>` being either `windows`, `mac` or `linux`

If the compiler gives an error saying that hxCodec cannot be found read this issue to fix it: ShadowMario/FNF-PsychEngine#12770

## Customization:

if you wish to disable things like _Lua Scripts_ or _Video Cutscenes_, you can read over to `Project.xml`

inside `Project.xml`, you will find several variables to customize Stellar Engine to your liking

to start you off, disabling Videos should be simple, simply Delete the line `"VIDEOS_ALLOWED"` or comment it out by wrapping the line in XML-like comments, like this `<!-- YOUR_LINE_HERE -->`

same goes for _Lua Scripts_, comment out or delete the line with `LUA_ALLOWED`, this and other customization options are all available within the `Project.xml` file

## Credits:

### Stellar Engine

- CharlesCatYT - Main Programmer

### Stellar: Special Thanks

- TheWorldMachinima - Softcoded Achievements
- notweuz - The features I took from OS Engine cuz im lazy rn

### Psych Engine

- Shadow Mario - Main Programmer
- RiverOaken - Artist

### Psych: Special Thanks

- bbpanzu - Ex-Programmer
- CubicYoshi/Yoshubs - Ex-Programmer, New Input System
- SqirraRNG - Crash Handler and Base code for Chart Editor's Waveform
- KadeDev - Fixed some cool stuff on Chart Editor, FPS Rainbow and other PRs
- iFlicky - Composer of Psync and Tea Time, also made the Dialogue Sounds
- PolybiusProxy - .MP4 Video Loader Library (hxCodec)
- Keoiki - Note Splash Animations
- Smokey - Sprite Atlas (Adobe Animate 2015-only) Support
- superpowers04 - LUA JIT Fork and some Lua reworks

---

# Features

## Mod Support

- Probably one of the main points of this engine, you can code in .lua (and .hx) files outside of the source code, making your own weeks without even messing with the source!
- Comes with a Mod Organizing/Disabling Menu.

## Cool new Chart Editor changes and countless bug fixes

- You can now chart "Event" notes, which are bookmarks that trigger specific actions that usually were hardcoded on the vanilla version of the game.
- You can manually adjust a Note's strum time if you're really going for milisecond precision
- You can change a note's type on the Editor, it comes with several example types:
  - Alt Animation: Forces an alt animation to play, useful for songs like Ugh/Stress
  - Hey: Forces a "Hey" animation instead of the base Sing animation, if Boyfriend hits this note, Girlfriend will do a "Hey!" too.
  - Hurt Notes: If Boyfriend hits this note, he plays a miss animation and loses some health.
  - GF Sing: Rather than the character hitting the note and singing, Girlfriend sings instead.
  - No Animation: Character just hits the note, no animation plays.

## Multiple editors to assist you in making your own Mod

![Screenshot_3](https://user-images.githubusercontent.com/44785097/144629914-1fe55999-2f18-4cc1-bc70-afe616d74ae5.png)

- Working both for Source code modding and Downloaded builds!

## Story mode menu rework:

![](https://i.imgur.com/UB2EKpV.png)

- Added a different BG to every song besides Tutorial.
- All menu characters are now in individual spritesheets, makes modding it easier.

## Credits menu

![Screenshot_1](https://user-images.githubusercontent.com/44785097/144632635-f263fb22-b879-4d6b-96d6-865e9562b907.png)

- You can add a head icon, name, description and a Redirect link for when the player presses Enter while the item is currently selected. You can even make a credits.txt file for your own mod credits.

## Awards/Achievements

- The engine comes with 16 example achievements that you can mess with and learn how it works. There's also softcoded achivement support by the way, by the creator of SScript.

## Options menu:

- You can change Note colors, Delay and Combo Offset, Controls and Preferences there.
- On Preferences you can toggle Downscroll, Middlescroll, Anti-Aliasing, Framerate, Low Quality, Note Splashes, Flashing Lights, etc.

## Other gameplay features:

- Lag doesn't impact the camera movement and player icon scaling anymore.
- You can reset your Score on Freeplay/Story Mode by pressing the R key.
- You can listen to a song or adjust Modifiers/Gameplay Changers on Freeplay by pressing Space.
- You can enable "Combo Stacking" in Gameplay Options. This causes the combo sprites to just be one sprite with an animation rather than sprites spawning each note hit.
