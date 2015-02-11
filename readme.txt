Operating in linux£º
1.Change to root mode using "su" cmd.
2.Insert SD reader with SD£¬linux mounts device automatically. Using "umount /dev/XXX" to umount device. XXX is device's name.
3.Using "fdisk ¨Clu" to check disk device in linux.Normal it is dev/sdb.
4.Copy omap3-mkcard.sh to linux system£¬add execute mode using "chmod +x omap3-mkcard.sh"£»"./omap3-mkcard.sh /dev/sdb" to part SD.
5.Go to /mnt directory£¬mkdir mmc1£»mount /dev/sdb1p0 mmc1.
6.Copy MLO uEnv.txt u-boot.img am335x-boneblack-bitmainer.dtb uImage.bin and initramfs.bin.SD to /mnt/mmc1 directory.
7.Umount /mnt/mmc1.
Only step 5, 6 and 7 are necessary, if SD is partitioned.
