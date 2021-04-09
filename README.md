# Artec T18AR V2.0.2.5 Windows Drivers and Software for USB QAM TV Tuner 

This repository contains the official driver files and software taken from the original CD that was included with the Artec T18AR HDTV USB Tuner.

I wasn't able to find this software anywhere online, so I decided to upload it to GitHub once I found my driver and software CD (this was the hardest part).

I hope these files help someone out there!  

## Windows 7

I wasn't able to get the ArtecMedia Digital TV Player application to work properly in Windows 7 x64.  I could watch TV, but there wasn't any sound despite the sound not being muted and at full volume.

I did get Windows Media Center to work propertly (sound and picture) with this HD TV USB adapter though.  You may need to un-plug and re-plug in this TV tuner adapter to get it work properly at times.  If Windows Media Center is unable to scan TV channels, unplug the USB adapter, plug it back in, and then try scanning for channels again.

I did run into a problem with Media Center downloading TV files, and I fixed it using this information:

https://www.yournearestbar.com/?tag=downloading-tv-setup-data

```
Given certain circumstances, Windows Media Center will get stuck at “Downloading TV Setup Data” and do nothing else. This generally occurs after some sort of hardware change, as it happened to me on a motherboard change and on a hard drive change. YMMV.

For the sake of clarity, this entire post refers to Windows 7, but it could apply to Vista as well, given that the paths are relatively the same.

Anyway, there are a few posts around the Web that tell you to run a command line for mcupdate.exe with some switches. That’s like getting a tire patch, it’ll work for now but won’t last. Here’s the new tire solution:

1) Go to the Control Panel, Programs and Features, and click “Turn Windows Features on/off”. Uninstall Windows Media Center.

2) Reboot.

3) Empty out the folder C:\ProgramData\Microsoft\eHome\

4) Go to the features and enable Windows Media Center again.

5) Run Windows Media Center and do the TV setup.

This solution is the only one that worked across reboots and allowed me to go and reset the TV signal without hassle. Please leave a comment if something else worked for you.
```

## Linux

It looks like this TV Tuner isn't supported at all by Linux.  I tried getting VLC and other media players to work with this card, but it doesn't seem possible to get it to work.
