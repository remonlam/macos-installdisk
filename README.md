# Create a bootable USB drive to install macOS (Sierra)

### Pre-requirements

## USB drive
Preferable a USB3 drive (because of speed) with 8GB (recommended, more is not required) of storage

## Download sources
Download Sierra from the Apple Store (this could take some time, the file is about 5GB big)

## Format USB drive
+ Mac OS Extended (Journaled)
+ GUID Partition Map
+ Name the disk (in my example I named it: Install macOS Sierra)

## Create the boot disk
Open Terminal and copy paste the command below

NOTE: Make sure you change the disk name if you named the disk different from the example below!


```shell
 sudo /Applications/Install\ macOS\ Sierra.app/Contents/Resources/createinstallmedia --volume /Volumes/Install\ macOS\ Sierra/ --applicationpath /Applications/Install\ macOS\ Sierra.app --nointeraction
 ```

Depending on the speed of your USB disk, this step could take up to 30 minutes to complete...

## Booting from the USB disk
Reboot or start your mac and hold down the "Option" key until you see a boot menu and select the USB disk


## Example output;

```shell
sudo /Applications/Install\ macOS\ Sierra.app/Contents/Resources/createinstallmedia --volume /Volumes/Install\ macOS\ Sierra/ --applicationpath /Applications/Install\ macOS\ Sierra.app --nointeraction
Password:
Erasing Disk: 0%... 10%... 20%... 30%...100%...
Copying installer files to disk...
Copy complete.
Making disk bootable...
Copying boot files...
Copy complete.
Done.
```
