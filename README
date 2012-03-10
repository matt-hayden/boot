

The util.lst has a few uncommon boot and rescue options. You can place a label
file 'bootme' in the root of a partition and util.lst has an option to find 
that partition and try booting. Backups of MBRs named hda.mbr or sda.mbr can be
loaded as well.


Hard drive installation notes

Install grub4dos to MBR with bootlace.com (works under DOS, Win9x or Linux)

Windows XP boot.ini may reference GRLDR by adding:
	C:\GRLDR="Grub4dos"
Without GRLDR, Windows will give an erroneous error message about missing
hal.dll.

Grub2 grub.cfg may reference the grub4dos grub.exe by adding:
	menuentry "Grub4dos"{
	setroot=(hd0,1)
	linux /grub.exe
	}


Boot sectors and disk images included:

freedos images: MSDOS replacement
	http://www.fdos.org/bootdisks/
	http://www.fdos.org/bootdisks/autogen/FDSTD.288.gz

gpxe: Internet boot Linux distributions
	http://boot.kernel.org (might be down)
	http://boot.kernel.org/gpxe_images/gpxe.lkrn
	This is a Linux kernel image.
	
hdt: Hardware diagnostic
	http://hdt-project.org/
	http://hdt-project.org/raw-attachment/wiki/hdt-0.5.0/hdt-0.5.0.img.gz
	This is a gzipped 1.44 MB floppy image

invaders: game
	http://www.erikyyy.de/invaders/
	http://www.erikyyy.de/invaders/invaders-1.0.0.tar.gz
	
memtest86: memory tester
	http://www.memtest86.com/
	http://www.memtest86.com/memtest86-4.0a.usb.tgz
	memtest86-4.0a.usb

memtest86+: memory tester
	http://www.memtest.org/#downiso
	http://www.memtest.org/download/4.20/memtest86+-4.20.bin.gz

netboot: Internet boot Linux distributions
	http://www.netboot.me/gettingstarted
	http://static.netboot.me/gpxe/netbootme.dsk

plop: boot manager
	http://www.plop.at/en/bootmanager/index.html
	http://download.plop.at/files/bootmngr/plpbt-5.0.14.zip
	plpbt.bin
	You may want to copy the PCMCIA directory into /Boot
	
sbm: boot manager
	http://paulski.com/zpages.php?id=1612
	sbm.img
	This is a 640K floppy image

smart boot manager:
	http://sourceforge.net/projects/btmgr/
	
##############################################################################
### Customized disks
### Show uuids with the uuid command. This can be useful with the following
### entries:
##############################################################################

title 72GB USB boot partition
uuid FC3C-A6CD
chainloader +1

title 72GB USB NTFS partition
uuid 462447F92447EA8F
chainloader +1