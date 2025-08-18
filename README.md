# Important!
Due to uncertainty about copyright issues, I do not provide the game files that are **absolutely necessary** to play the game. They used to be available at http://update1.baiyou100.com/resource/Pal98rqp.zip , but the forum is no longer up, so the link doesn't resolve. You can find the same files on the *internet* in a certain *archive*

## List of distros where the game works as expected using the binary:

![Static Badge](https://img.shields.io/badge/CentOS_Stream_10-purple)

## How to play one of the longest running, most influential eastern RPG series' first entry 
### This tutorial assumes you are trying to play the game on a Linux/Unix system
As I don't use Windows or MacOS, I do not have pre-built binaries for it - see the additional resources for links to the original repo, where you can find build instructions for your system of choice.

To play the game on a modern system, you will need 3 things (2 if you can read Chinese):
1. The original game files (not provided, see above)
2. The english patch
3. SDLPAL

Additional external resources are linked at the bottom of the page.

### Getting started
1. Unzip the game data archive to somewhere, you would like the game files to be - a good place could be for example `~/games`
   - create the directory if needed `mkdir -p ~/games`  
2. Download the binary from this repository, and move it into the directory the game data is in
   - `mv sdlpal ~/games/game_data_dir`
3. Move everything from the translation patch into the game data directory - overwrite existing files if needed
   - `mv xyz ~/games/game_data_dir`
4. From the game data directory, launch the binary
   - `./sdlpal`
5. If it's the fist time launching the game, a config window will show up - make sure to write the path to your english patch file in the correct field
   - by default it should be `./win_files/m_eng.sfl`
6. The setup is now complete - enjoy the game!

### Optional steps
#### Create a desktop shortcut
On Gnome, you can easily create a shortcut:
1. Use your favourite text editor to create a new desktop file
 
     `nano ~/.local/share/applications/sdlpal.desktop`
2. Paste the following, replacing the path to the executable and the icon if needed
     ```
     [Desktop Entry]
     Name=Chinese Paladin
     Terminal=False
     Comment=Play Chinese Paladin
     Type=Application
     Category=Game
     Exec=~/games/game_data_dir/sdlpal
     Icon=~/games/game_data_dir/logo.ico
     ```
3. If it doesn't appear, you may need to logout and log back in

### Additional resources
[Chinese Paladin on Wikipedia](https://en.wikipedia.org/wiki/The_Legend_of_Sword_and_Fairy)

[Chinese Paladin fansite with the original instructions](https://chinesepaladin.org/download-play-the-legend-of-sword-and-fairychinese-paladin-game-in-english/)

[English patch on romhacking.net](https://www.romhacking.net/translations/2441/)

[The original SDLPAL repository with source and build instructins](https://github.com/sdlpal/sdlpal)

### TODO

- Pictures
- Test on more distros, wsl, bsd, solaris
- Shortcut instructions for other desktop environments
- matrix room for support and general conversation
