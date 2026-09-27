# Installation

## Requirements

- 4GB RAM
- 64-bit CPU (at least 1GHz speed)
- 20GB storage (40GB recommended)

### ISO Setup
1. Download the ISO from Sourceforge.
2. Write the ISO to any USB drive u have available (at least 4GB - remember, everything will be wiped) using something like Rufus On Windows, balenaEtcher on Linux or just generally use Ventoy.

### Booting the ISO
1. Go to your BIOS/UEFI boot menu and select the USB drive you used.
2. Select the first option in GRUB (second entry is for if you have issues with your GPU, so it uses the kernel option 'nomodeset'.).
3. When done, the live environment should automatically log you in and start Calamares.

### Installing Infinity Linux with Calamares
1. When Calamares starts, make sure you have <b>at least one</b> disk or partition you want to use, or Calamares will not continue. When you're sure of this, click Next.
2. Select your region/timezone and keyboard layout and continue.
3. When asked to choose whih options to use on the partition page(if you look carefully, there is an option above to choose which disk u want to use. Please select the one you want to use for this to avoid complications), use the options you see as explained:
- Replace a partition: If you have a dedicated partition you want to use, select this option and click on the partition you want to replace or wipe.
- Wipe the whole disk: This is ideal if you want to use your whole disk for Infinity Linux. It's advisable to use a swap partition with this or just swap to file.
- Shrink partitions: If you want to install this alongside another linux distro, it's ideal to shrink the partition to your desired size, select it, and continue. (NOTE: DON'T RESIZE NTFS PARTITIONS WITH THE INSTALLER! YOU MIGHT RENDER YOUR WINDOWS INSTALLATION UNUSABLE. USE AT YOUR OWN RISK!)
- Manual partitioning: This is for manual control over the partitions you want to use for the OS. Mountpoints include:
	- /efi: for EFI partition, must be 1GB and formatted with FAT16/FAT32.
	- /: Root filesystem, can be formatted with Ext4, btrfs,  jfs, xfs, or other POSIX-compatible filesystems. Please note that NTFS will not work.
- When done with all this, you can proceed.
4. Enter the username and password you want to use. It's recommended to deselect 'Use the same password for the admin account' to keep away unaiuthorized usage of root superuser with your main password. Proceed when finished.
5. Now, go through everything on this page clearly. If everything is in order, click Install. If something feels off, you can always go back and check.
6. Watch as it finishes installing. You can play around with the live environment while you wait. When it's done, you can reboot the system.

<h3>Congratulations! If you're done with everything here, you can proceed to the next item on the list.</h3>

