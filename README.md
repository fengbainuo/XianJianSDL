# Chinese Paladin - The Legend of Sword and Fairy

# Important!
Due to uncertainty about copyright issues, I do not provide the game files that are **absolutely necessary** to play the game. They used to be available at http://update1.baiyou100.com/resource/Pal98rqp.zip , but the forum is no longer up, so the link doesn't resolve. You can find the same files on the *internet* in a certain *archive*

You can also - and this is the recommended way - buy the game on Steam. As it has never been officially released in the west, the Steam version is only available in Chinese. That's fine however, you only need the game data, the translation is available in this repository.

## List of distros where the game works as expected using the binary:

![Static Badge](https://img.shields.io/badge/CentOS_Stream_10-purple) ![Static Badge](https://img.shields.io/badge/Debian%2013-blue)
 ![Static Badge](https://img.shields.io/badge/WSL-Ubuntu%2024.04-orange)

## How to play one of the longest running, most influential eastern RPG series' first entry 
### This tutorial assumes you are trying to play the game on a Linux/Unix system
As I don't use Windows or MacOS, I do not have pre-built binaries for it - see the additional resources for links to the original repo, where you can find build instructions for your system of choice.

To play the game on a modern system, you will need 3 things (2 if you can read Chinese):
1. The original game files (not provided, see above)
2. The english patch
3. SDLPAL

Additional external resources are linked at the bottom of the page.

### Prerequisites for WSL2 users
Assuming you are using the default Ubuntu WSL, you need the following two packages:
   ```
   sudo apt-get install libsdl2-dev
   sudo apt-get install libxft2
   ```

### Getting started
1. Unzip the game data archive to somewhere, you would like the game files to be - a good place could be for example `~/games`
   - create the directory if needed `mkdir -p ~/games`
     
   ![Screenshot showing the archive and the unzipped directory](https://github.com/fengbainuo/XianJianSDL/blob/main/sdlpal_screenshots/Screenshot%20From%202025-08-18%2016-34-16.png)
2. Download this repository and copy the following files to the game data directory - overwrite existing files if needed:
   - **SDLPAL binary:**
      - `cp -pv sdlpal ~/games/game_data_dir/`
   - **Translation patch:**
      - `cp -prv paleng_v3.3/* ~/games/game_data_dir/`
5. From the game data directory, launch the binary
   - `./sdlpal`
6. If it's the fist time launching the game, a config window will show up - make sure to write the path to your english patch file in the correct field
   - if you followd the steps until now, you can leave the first line as it is
   - by default the localization files location should be `./win_files/m_eng.slf`

     ![Screenshot showing the config menu](https://github.com/fengbainuo/XianJianSDL/blob/main/sdlpal_screenshots/Screenshot%20From%202025-08-18%2016-35-48.png)
7. The setup is now complete - enjoy the game!

   ![Screenshot showing the main menu of the game](https://github.com/fengbainuo/XianJianSDL/blob/main/sdlpal_screenshots/Screenshot%20From%202025-08-18%2016-36-52.png)
   ![Screenshot of the game running under WSL](https://github.com/fengbainuo/XianJianSDL/blob/main/sdlpal_screenshots/Screenshot%20From%202025-08-18%2018-29-09.png)
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
     Icon=~/games/game_data_dir/Logo.ico
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
