Sash
====

Stand-alone shell, which has several utilities built into it. Ideal for rescuing a system as it is statically compiled.

Source: http://members.canb.auug.org.au/~dbell/programs/

The "plus patches" version (marked as `*-fmb`) adds `chroot`, `pivot_root`, and `losetup` to versions 3.5 through 3.7. I've also backported it to 3.4. As of version 3.8, those patches are included by the original maintainer.

Sash plus patches: http://www.baiti.net/sash/


Build Notes
-----------

3.4 - Changed the include from `linux/ext2_fs.h` to `ext2fs/ext2_fs.h`. be79adb

3.4-fmb - Altered the 3.5 patch to work with the older version.

3.5 through 3.7 - Cherry picked the header include change from 3.4.

3.8 - Cherry picked the header include change from 3.4. This version contains the "plus patches" already.
