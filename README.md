# mac-boot
An application to allow Apple machines to PXE boot to FOG

This application is meant to make mac pxe booting into FOG easier of OS X.  It supports both 32 and 64 bit EFIs.  The installer creates a partition for the files to reside.  Due to limitations in OSX the smallest the partition can be is around 700mb.  A bit much for only 15mb or so.

Attention 32bit EFI users must install the CSM(BIOS) version of the software.  This involves creating the nasty Hybrid MBR.  Because 32 EFI on Apple computers do not reveal their network devices to iPXE we have to fall back to the BIOS version.  Because of this it is strongly recommended that you create a backup of your device before installing Mac-Boot.

The above warning also pertains to 64bit EFI users that select "Install Both Versions."  

The latest version also supports creating external bootable USB for 64bit EFIs and CD's for 32 bit EFIs
