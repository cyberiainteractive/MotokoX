# Modifications

Keeping track of the source files I've modified.

## Main Menu
- [x] Oni_InGameMenu.c, Oni_OutGameMenu.c, Oni_MenuNav.c, Oni_MenuNav.h, WM_Dialog.c

These were rewritten to allow menu navigation via the controller, a feature that's sorely missing from the initial source code. If you're porting Oni to another video game console, I'd recommend taking a look at it and seeing if it suits your needs! Rockstar Canada didn't feel the need to iterate that much on the PC menu, and neither do I.
- [x] Oni_Persistance.c

This has been modified to save persist.dat (Oni's config + save file) in E:\UDATA\4D530012, create and copy the appropriate TitleMeta.xbx and TitleImage.xbx files on first run, and create the appropriate SaveMeta.xbx and copy over the appropriate SaveImage.xbx at every save point, so the game feels like a native console port and can be run from XISO, CD/DVD or HDD. This also inadvertently fixes an issue in OniFoxed where settings and save data won't save by default unless "persist.dat" is created first.

## Oni
- [x] level0_Final.dat - Extracted, rewrote and repacked SUBTmessages to replace global keyboard input names with Xbox button name equivalents.
