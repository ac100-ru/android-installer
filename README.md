android-installer
=================

Auxilary scrypt for CM11 installation
For more information about CyanogenMod for AC100 see [project page](http://code.google.com/p/cm-paz00/).

Installation
--------------

1. Download [cm_ac100-ota-11.0-20140322-UNOFFICIAL.zip](https://docs.google.com/uc?export=download&confirm=xQ1b&id=0BzHUnWusu2ztdjZjRmE3VW9YWlk), [gapps-4.4.2_20​140110.zip](http://yadi.sk/d/tkRraxinKCtpZ) and [recovery-11.0-20140322.img](https://drive.google.com/uc?id=0BzHUnWusu2ztc3R2OEEta19sYzA&export=download)

2. Download [installer](https://raw.githubusercontent.com/ac100-ru/android-installer/master/installer)

3. Put downloaded files (.zip, .img, installer) into the **root folder** of SD card or USB flash drive (first partition). Don't foget to safely remove the SD card/USB flash drive from a PC.

4. Download [sos-uboot](https://dl.dropboxusercontent.com/u/40761340/Test/sos-uboot-r5-2014-07-01.bin)

5. Start AC100 in recovery mode :
    `hold Ctrl+ESC keys while pressing Power during boot`

6. Run sos-uboot :
    `./nvflash --bl sos-uboot-r5-2014-07-01.bin --go`

7. Insert the SD card/USB flash drive into AC100

8. Mount source :
    `mount /dev/sda1 /mnt`

9. Run installer :
    `sh /mnt/installer`
