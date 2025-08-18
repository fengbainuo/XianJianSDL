======================
[Instructions]
======================
##########
ENG Installation Instructions / 繁體安裝說明 (CHT) / 简体安装说明 (CHS)
##########

0. (optional) Backup a copy of your original 'm.msg', 'sss.mkf', 'word.dat'. Additional files 'wor16.asc', 'wor16.fon' for PalDOS.
1. Overwrite the extracted files for your GAME VERSION into the game directory.
2. [For Microsoft Windows platform], copy the included win32 'sdlpal.exe' version into the game directory
	- For latest updates and other platforms, download @ official SDLPal page: https://github.com/sdlpal/sdlpal with the 'Download' button @ README.md section
	- For touch-based only platforms, change this line 'UseTouchOverlay=0' to 'UseTouchOverlay=1' in 'sdlpal.cfg' file
3. (optional) Documentation of 'sdlpal.cfg' options: https://github.com/sdlpal/sdlpal/blob/master/docs/sdlpal.cfg.example


##########
Additional Instructions for Other Languages / [續] 繁體安裝說明 (CHT) / [续] 简体安装说明 (CHS)
##########

4. Edit 'sdlpal.cfg' file @ line 'MessageFileName=m_eng.slf' to read the desired language file, e.g. 'm_cht.slf'/'m_chs.slf'.


======================
[Credits]
======================
Xire and unmentioned translators for Original Translation (v2.5)
chamine for 'PalDialogs Tool'
Pantamorph and others for keeping the original translated files alive
Administrators for maintaining Chinese Paladin English Forum @ http://fairysword.windy-goddess.net/phpBB/index.php

Whistler for the original 'SDLPal'
SuperMouse (louyihua) and SDLPal team for 'SDLPal International'/Unicode Support fork & merge
PalMusicFan for the many assistance in making SDLPal translation port possible


======================
[Hotkeys]
======================
General
Enter/Space/Numpad Enter - Ok/Search/Speak
Esc/Insert/Alt/Numpad 0 - Menu/Cancel

Skill/Item Menu
Page Up		- Scroll Up 1 Page
Page Down	- Scroll Down 1 Page
Home 		- First Item (SDLPal only)
End			- Last/Newest Item (SDLPal only)

Adventure-specific shortcuts
Q - Quit Game
W - Equip Item
E - Use Item
S - Status Screen
F - Spell

Battle-specific shortcuts
Q - Flee Battle
W - Use Projectiles
E - Use Item
R - Repeat Previous Command
A - Auto Attack Previous Enemy
S - Status Screen
D - Defend
F - Auto Spell Usage (Strongest)


======================
[Changelog]
======================
v3.3 20190831 (by Nostaljaded)
- Fixed dialog text styling due to new symbols (not present in original game) being used for text styling (by other mods) in recent SDLPal
- Renamed localization filename extension to SLF (SDLPal Localization File)
- Renamed Lao Lao to Grandma, Miss Liu to Madam Liu, Chief Priestess to Queen, A Nu to Ah Nu, Mentor to Master Ling Yue & other minor characters
- Fixed NPCs not properly named for a village in the latter half
- Another pass on minor text cleanups for more faithful translation
- Other minor text cleanups @ 55%

v3.2 20171231 (by Nostaljaded)
- Included win32 SDLPal mingw build
- Simplified other language installation instructions
- Updated SDLPal official sourcecode link & other links
- Renamed win_files filenames to follow freeware filename conventions
- Merged desc.dat into language file, now all localization is in 1 single file
- Fixed CHS & CHT Equip & Status screen layout and illegible font size
- Other minor text cleanups @ 50%

v3.1 20151231 (by Nostaljaded)
- SDLPal DOS ENG support (applicable only to SDLPal, not motivated to copy over 10k lines line-by-line for original PalDOS support)
- Cross-referenced and corrected original Chinese dialog lines in DOS & WIN (applicable only to the SDLPal externalized message file to serve as base for modding and other language translations)
- Refactored Equip & Status screen layout to accommodate long item names (applicable only to SDLPal)
- Translated poison bugs item descriptions (leftover from v3.0)
- Translated Chinese poetry (one more)
- Replaced inbattle status with symbols due to 3 character limits
- Renamed lesser NPCs' names in Pinyin format to be consistent with main characters
- Other minor text cleanups @ 40%

v3.0 20150731 (by Nostaljaded)
- Blind proofread and edit (translation shenanigans continues with their tribal dance, Ugachaka U!)
- Translated Chinese poetry (a few)
- Replacement of item/spell acronyms with partial adoption of Last Fencer's better item/spell names

v2.5
- Changed skill name "Berserk"&"Debuff" to "Confuse"&"Dispel" and fixed skill description of Nu Wa transformation.
- Full item explanations/descriptions (nearly everything except poison bugs)

v2.1
- Fixed crash while talking to a White Miao close to Da Li.
- Fixed some spelling mistakes
- More accurate translation
- Added skill names of each character/+ more item descriptions

v1.2
- Fixed crash after fighting with Black Miao Elder
- Fixed crash while Yueru is explaining Liu's background to Xiaoyao


======================
[Untranslated/Outstanding Stuff]
======================
- Text overflows may occur as dialogs not revised for character count and/or checked for translation quality (Stopped @ PalWIN 'Don't... you have relatives?' & checked from 'This door is locked' to the end)
- Some item/spell names could have a better translation
- Some rhymes & opera lines (non-critical to main plot) remained in the original Chinese format


======================
[Comments, feedbacks, suggestions]
======================
- http://fairysword.windy-goddess.net/phpBB/viewforum.php?f=3 (Not a member there, will occasionally pop by to check new posts)
- http://www.rpgcodex.net/forums/index.php?threads/the-legend-of-sword-and-fairy-aka-chinese-paladin.99662/ (if you have what it takes)


======================
[Small Talk]
======================
- Play the PalDOS version for its original dungeon layout and monster difficulty level. You are forewarned as some replaying players still lose their way in the latter dungeons for PalWIN version.

- This translation is NOT a high-quality translation, unlike some other fan-translated games; so keep your expectations DOWN.

- Instead of the original executable, use the included win32 SDLPal executable or get the latest release @
	Official SDLPal source code repository: https://github.com/sdlpal/sdlpal with the 'Download' button @ README.md section
	(Ongoing code features & bug commits)
	+ Internal Unicode font support
	+ Flexible dialog lines & additional dialog text styling colors support
	+ Longer skill & item names support
	+ Externalized hardcoded text in Equip menu
	+ Editable Equip & Status screen layout
	+ Resizable game window size
	+ Stereo RIX & other formats audio support
	+ Individually adjustable Music & FX volume
	+ Native gamepad support (Use 3rd-party keyboard mapping software for custom gamepad layouts)
	+ Touch-based support
	+ Savegame compatible with the official Pal.exe
	+ Other adjustable options in sdlpal.cfg
	+ Multi-platform support
	+ [PalWIN] No forced change of Desktop Color Composition
	+ [PalDOS] Support Item & Spell infobox
	
- Valiant translation done by Xire and translators, probably his/her/their 1st translation project.
	~ Could be more structured though as there were (probably still have) nouns mismatched in different locations.
	~ Not a good idea to insert hints when original text does not have them; could be done in a FAQ file.
	
- 1T (tael, unit weight of silver) = 1,000G (coin)


##########
As Chinese is a very compact language, so there's bound to be lost-in-translation (formerly due to character width limitations, now alleviated by SDLPal).
##########
An extended translation of the actual opening scene is implemented in SDLPal to showcase flexible dialog lines feature.

Alternate longer version when Ling'er sings softly at night, implemented in SDLPal as well.
既不回頭，何必不忘；
既然無緣，何需誓言。
今日種種，似水無痕，
明夕何夕，君已陌路。

[Original]
Leave me with the passing day,
Fate'll break the promise you made.
Today is a dream flowing away,
Morn, we'll be on separate ways.

[SDLPal]
You ain't returning, why remember me?
We ain't meant to be, why make promises?
Today will just be sweet memories;
Come tomorrow, we'll just be strangers.


++++++
So, how much could be improved?
++++++
Here's a current sample:
# 李逍遙：
# 怎麼會可憐？
# 我反倒覺得劉兄最幸福呢！
# 有這麼一個漂亮又賢淑的妻子
# 天天照顧他，要是我也娶到這
# 種老婆，作鬼也甘願呢！
Li Xiaoyao:
Why pity?
I think he is lucky for having
such a beautiful wife taking
care of him. I wish I can
marry such wife too.

# 林月如：
# 那你就去死一死吧你
# 去讨个女鬼当老婆！
Lin Yueru:
You better go
to hell now!


Enjoyz,
Nostaljaded

P.S. May the better/other language translators step forward to bring this game to a wider audience.
Good games are meant to be shared.