# BBS
Blank-Board-Serializer used to burn SN into blank logic board (for Apple org boards only)

First create bootable USB memory stick:

# from mac os command line:

$> cd ~/Downloads                                   # move to folder with BBS_

$> hdiutil convert bbs.dmg -format UDTO -o bbs.iso  # create bootable iso image

 insert USB memory stick into USB port and look after /dev/disk<number> using
  
$> DiskUtility list

 Create bootable USB using ISOimage file and USB drive 

$> sudo dd if=bbs.iso of=/dev/disk<number> bs=10m
  
 With this bootable USB memory stick power up your mac with alt-option key pressed

 when images with bootable disks shows up then select BBS

 folow the instructions and enjoy your serialized mac!

