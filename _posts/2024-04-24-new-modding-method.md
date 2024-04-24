---
layout: post
title: Back 4 Blood - The Final Modding Method
subtitle: Hopefully, anyway...
tags: [back4blood]
comments: false
---

Thanks to internet famous UE modder trumank, we finally have a method of patching the game with the old .pak file format. This means no more unpacking!

Everything previously applicable holds true except:
- Instead of unpacking and running the game with -nopak, leave the game packed and run the game with -fileopenlog
- When creating a mod, instead of packing with UnrealPak, you should use this [custom tool created by trumank](https://smooversyt.github.io/downloads/repak_b4b.exe).

To use the new tool:
1. Place the tool in the same directory as the root folder of your mod (the one above Gobi).
2. Create a new text file in the same directory.
3. Name the file Repak.bat
4. Edit the file to contain this: repak_b4b.exe pack --version V9 \<mod_name\>
5. If all goes well, you should see a command prompt open, run, and then close, leaving behind your .pak file in the same directory.

To install new mods from scratch:
1. Locate your Back 4 Blood install directory. You can do this on Steam by right-clicking Back 4 Blood on the left side of your library and clicking Manage > Browse Local Files.
2. Navigate to /Back 4 Blood/Gobi/Content/Paks.
3. Extract your downloaded zip file into the Paks folder.
4. Go back to Steam and right-click on Back 4 Blood on the left side of your library and click Properties.
5. In the Launch Options box, type: -fileopenlog

A lot of our old mods have been updated and posted to Nexus [here](https://www.nexusmods.com/back4blood/mods/).

Have fun!

PS: I've been informed that the site to download quickbms is down, so [here's a download](https://smooversyt.github.io/downloads/quickbms.zip) including the B4B specific script for unpacking.