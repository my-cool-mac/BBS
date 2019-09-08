# BBS
Blank-Board-Serializer used to burn SN into blank logic board (for Apple org boards only, models 2019 inclusive)

First, after you. downloaded this repo & unzip iso file - create bootable USB memory stick:


# From mac os command line:


[1]$> cd ~/Downloads                                   # move to folder with downloaded BBS* files


if you want to create your own BBS.iso file [2] else [3]:

[2]$> hdiutil convert BBS.dmg -format UDTO -o BBS.iso  # create bootable iso image


Insert USB memory stick into USB port and look after /dev/disk[number] using
  
[3]$> diskUtility list


Create bootable USB using ISOimage file and USB drive 


[4]$> sudo dd if=bbs.iso of=/dev/disk[number] bs=10m

  
With this bootable USB memory stick power up your mac with alt-option key pressed

when images with bootable disks shows up then select BBS

follow the instructions and enjoy your serialized mac!
