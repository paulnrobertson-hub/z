# Lyrics 3D (Fabric, Minecraft 1.21.11)

Shows the lyrics of whatever you're playing as floating 3D text in front of you.
Works with Spotify, and YouTube / SoundCloud in a browser (Windows 10/11 only).

## Build the .jar (easiest: GitHub)
1. Make a free GitHub repo and upload everything in this folder (keep the .github folder).
2. Open the repo's **Actions** tab -> **build** -> **Run workflow**.
3. When it finishes, download **lyricsmod-jar** and unzip it. That .jar is the mod.

## Build on your own PC instead
Install JDK 21 and Gradle 9.2, then in this folder run: `gradle build`
The mod is in `build/libs/lyricsmod-1.0.0.jar` (not the -sources one).

## Install
Put the .jar and **Fabric API** (0.141.1+1.21.11) in `.minecraft/mods`, launch with Fabric Loader.

## Use
Play a song, then join a world. Commands:
- `/lyrics` turn on/off
- `/lyrics distance <1-12>` how far in front of you (default 3.5)
- `/lyrics height <-3..3>` move up/down (default 0.4)
- `/lyrics offset <ms>` fix sync; positive shows lyrics earlier

Lyrics come from lrclib.net. Songs without synced lyrics there show "No synced lyrics found".
