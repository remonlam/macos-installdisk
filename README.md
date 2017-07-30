# Create a bootable USB drive to install macOS (Sierra)

### Pre-requirements

## USB drive
Preferable a USB3 drive (because of speed) with minimal 8GB of storage

## Download sources
Download Sierra from the Apple Store (this could take some time, the file is about 5GB big)

## Format USB drive
+ Mac OS Extended (Journaled)
+ GUID Partition Map
+ Name the disk (in my example I named it: Install macOS Sierra)

## Create the boot disk
Open Terminal and copy paste the command below

NOTE: Make sure you change the disk name if you named the disk different from the example below!


``` sudo /Applications/Install\ macOS\ Sierra.app/Contents/Resources/createinstallmedia --volume /Volumes/Install\ macOS\ Sierra/ --applicationpath /Applications/Install\ macOS\ Sierra.app --nointeraction ```
