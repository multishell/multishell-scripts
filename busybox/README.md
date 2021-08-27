BusyBox
=======

Initially, BusyBox did not start with a shell, but they soon added Lash in 0.43. After that, Ash, Msh, and Hush were included in 0.52. Lash and Msh were eventually dropped. This project builds all shells contained within BusyBox. Each shell will be a separate binary that defaults to running the shell.

Source: https://busybox.net/downloads/


Build Notes
-----------

0.25 - Changed extern into static. b0e39cd1 Removed `bdflush()`. 6810ed87 Swapping SIGUNUSED with SIGSYS. bd080b3d Changing `umode_t` into `__mode_t`. ab325f48 Sync does not return a value. 0b54bcd2 NO SHELL

0.43 - First version that has a shell. Fixed error during creation of documentation. 4259ba65 Defined `MINIX2_INODES_PER_BLOCK`. e6488fa0 Set default file mode for `open()`. 9ff96773 Made some `extern` variables `static` instead. 76a677d8 Removed `kdaemon.h` and `bdflush()` since it's now automatic since Linux 2.6. a68c94a2 Replace `SIGUNUSED` with `SIGSYS`. 21ebbb2e Removed casts and ternaries on the left hand side of assignments. dbfcd2f7 Removed unnecessary include `asm/page.h`. 0346f1dc Defined `NFS_VERSION`. 54a7d866 Updated `delete_module` system call. 45bd2dcd Updated `_llseek` system call and use `lseek` on 64-bit systems. 8044efef `sync` does not return a value. d5a56a03 Added `limits.h` for `PATH_MAX`. 07ade7a2 Switched away from `OPEN_MAX` and use `sysconf` to determine the value. 16b17d96 Runs the shell by default when invoked as `busybox-*`. fbac9b29

0.45 - Added `MINIX2_INODES_PER_BLOCK`, default file mode, and extern variables from 0.43. Updated `kdaemon.h` and `bdflush` patch. 721ec460 Replaced system calls in `insmod.c`. 8ee8a783 Added include file to get `EM_486` defined value. bcc94cba Added `SIGUNUSED`, casts, and `asm/page.h` fixes from 0.43. Updated `rmmod.c` system calls patch. 0e52649f Added `_llseek` patch from 0.43 Updated system calls in `swaponoff.c`. 15a9b8bd Updated seek returning no value patch. d2b42309 Updated system calls in `umount.c`. 2b175f46 Used `OPEN_MAX` from 0.43. Made the `next` function static for inlining. 539dedad Run shell by default from 0.43.

0.46 - Added default file mode and extern variables from 0.43. Added bdflush from 0.45. Replaced system calls in insmod.c. 964417c3 Used `EM_486` from 0.45. Used `SIGSYS`, removed casts, removed `asm/page.h` from 0.43. Updated system calls in `rmmod.c`. 3ea48a5f Updated system calls in `swaponoff.c`. f750668e Used `sync` patch from 0.45. Used `OPEN_MAX` from 0.43. Updated system calls in `utility.c`. e050a63b Used next function static from 0.45. Run shell by default from 0.43.

0.47 - Fixed multiline string in `cut.c`. 9748a4ca Used default file mode for open and extern variables patches from 0.43. Used bdflush patch from 0.45. Updated insmod system calls. b5f3509d Used `EM_486` patch from 0.45. Updated the removal of casts from left hand side of assignments. 18265ba7 Updated removal of `asm/page.h`. ab73409a Used system call updates for `rmmod.c` and `swaponoff.c` from 0.46. Used `sync` patch from 0.45. Updated `OPEN_MAX` patch. 542badbf Updated system call replacements in `utility.c`. 70c83a37 Applied the next function from 0.45. Updated patch to run the shell by default. bd9c0e95

0.48 - Updated multiline string patch for `cut.c`. 3f70f341 Updated default file mode for `gunzip.c` and `gzip.c`. e1f9718d Updated making variables `static` instead of `extern`. c1154179 Used `bdflush` from 0.45. Set up new defines for 64-bit machines in `insmod.c`. fb72c901 Used `insmod.c` system calls, removing casts, and removing `asm/page.h` patches from 0.47. Applied updated system calls in `rmmod.c` and `swaponoff.c` patches from 0.46. Applied `sync` patch from 0.45. Applied system call patch for `utility.c` from 0.47. Made next function static from 0.45. Updated running the shell by default. 54dc1148

0.49 - Updates system calls in `pwd_grp/setgroups.c`. 6ba666c1 Applied default file mode and extern variables from 0.48. Applied bdflush from 0.45. Applied `asm/page.h` from 0.47. Applied updated system calls for `swaponoff.c` from 0.46. Applied `sync` from 0.45. Applied system calls for `utility.c` from 0.47. Updated running the shell by default. 4137fa87

0.50 - Added default file mode and extern variables from 0.48. Added bdflush from 0.45. Removed `asm/page.h` from 0.47. Updated system calls for `mount.c`. e01c8ca5 Updates system calls for `swaponoff.c`. b048b0b1 Updated system calls in `utility.c`. 9eb1227d Run shell by default from 0.49.

0.51 - Updated system calls in `libbb/syscalls.c`. 844d0fca Made external variables static. 31340716 Set default file mode for `gzip.c`. 71e12930 Removed bdflush from 0.50. Removed `asm/page.h` from 0.47. Fixed conflicting types in `applets.c`. 6daf4fbf Added `query_module` to `libbb/module_syscalls.c`. 6e94feff Run shell by default from 0.49.

0.52 - First version that has ash, msh, lash, and hush as separate shells. Updated system calls in `libbb/syscalls` from 0.51. Set default file mode for gzip open and removed bdflush from 0.50. Removed `asm/page.h` from 0.47. Added `query_module` from 0.51. Updated running the shell by default. df93b9d2

0.60.0 - Format of `Config.h` changed for the multiple shells. Updated system calls in `libbb/syscalls` from 0.51. Set default file open mode from 0.50. Updated the removal of `bdflush`. ca24ed4a Removed `asm/page.h` from 0.47. Added `query_module` from 0.51. Run shell by default from 0.52.

0.60.1 - Updated system calls in `libbb/syscalls` from 0.51. Set default file open mode from 0.50. Updated the removal of `bdflush` from 0.60.0. Removed `asm/page.h` from 0.47. Added `query_module` from 0.51. Run shell by default from 0.52.

0.60.2 - Updated system calls in `libbb/syscalls` from 0.51. Set default file open mode from 0.50. Updated the removal of `bdflush` from 0.60.0. Removed `asm/page.h` from 0.47. Added `query_module` from 0.51. Updated running the shell by default. e3e191f6

0.60.3 - Updated system calls in `libbb/syscalls` from 0.51. Updated patch to set default file open mode in `gzip.c`. 3966e350 Updated the removal of `bdflush` from 0.60.0. Removed `asm/page.h` from 0.47. Added `query_module` from 0.51. Run shell by default from 0.60.2.

0.60.4 through 0.60.5 - Updated system calls in `libbb/syscalls` from 0.51. Applied default file open mode in `gzip.c` from 0.60.3. Updated the removal of `bdflush` from 0.60.0. Removed `asm/page.h` from 0.47. Added `query_module` from 0.51. Run shell by default from 0.60.2.

1.00-pre1 - Build system changed from `Config.h` to a config system. Set default file open mode for `archival/gzip.c`. 3edf66cf Removed unnecessary include of `asm/page.h` and defining `PAGE_SHIFT` in `libbb/procps.c`. d5707b3f Run the shell by default. bcba6258

1.00-pre2 through 1.01 - Applied open file mode, include file fixes, and running the shell as default from 1.00-pre1.

1.1.0-pre1 - Updated `Makefile` to remove `-e` for echo, which made `include/config.h` invalid. 7170857a Applied open file mode, include file fixes, and running the shell as default from 1.00-pre1.

1.1.0 - Fixed `include/config.h` generation from 1.1.0-pre1. Applied open file mode, include file fixes, and running the shell as default from 1.00-pre1.

1.1.1 - Fixed escaping of newlines in `scripts/config/mkconfigs`. 14478a07 Applied open file mode from 1.00-pre1. Use the system's `sysctl` instead of a local version. 15a610ee Avoid conflicting includes for `struct iphdr`. 53591474 Updated patch for `asm/page.h` and `PAGE_SHIFT`. 4f5b8587 Set default file mode in `e2fsprogs/ext2fs/ismounted.c`. 23f4588e Patched in system calls into `modutils/insmod.c`. 15bb29f4 Run shell as default from 1.00-pre1.

1.1.2 through 1.1.3 - Fixed newline escaping from 1.1.1. Applied open file mode from 1.00-pre1. Use system's `sysctl`, avoid conflicting includes, remove `asm/page.h`, set default file open mode, patch system calls from 1.1.1. Run shell as default from 1.00-pre1.

1.2.0 - Updated newline escaping. 0167d8ad Applied open file mode from 1.00-pre1. Use system's `sysctl` from 1.1.1. Fixed the conflicting `struct iphdr` patch. 39e82432 Removed `asm/page.h`, set default file open mode, and patched system calls from 1.1.1. Run shell as default from 1.00-pre1.

1.2.1 through 1.2.2 - Escaped newlines from 1.2.0. Applied open file mode from 1.00-pre1. Use system's `sysctl` from 1.1.1. Fixed conflicting `struct iphdr` from 1.2.0. Removed `asm/page.h`, set default file open mode, and patched system calls from 1.1.1. Run shell as default from 1.00-pre1.

1.2.2.1 - Escaped newlines from 1.2.0. Applied open file mode from 1.00-pre1. Use system's `sysctl` from 1.1.1. Fixed conflicting `struct iphdr` from 1.2.0. Removed `asm/page.h`, set default file open mode, and patched system calls from 1.1.1. Run shell as default from 1.00-pre1. Changed `EXTRA_VERSION` to make the version number different than 1.2.2. eca458b6

1.3.0 - Split `Makefile` rule definitions. 1114a503 Made functions inline to eliminate linking errors for `config`. f815ab28 Applied gzip open file mode from 1.00-pre1. Stopped erroring on warnings. 61f8a2a4 Set open file mode in ismounted.c from 1.1.1. Fixed function signatures. 1.3.0 Get `rlimit` struct. 4e8b0943 Get `rusage` struct. 9c02527c Get various resource structures and constants. 57b84181 Updated patch to use system-provided `sysinfo`. 79f6cafe Fixed conflicting `iphdr` from 1.2.0. Get `limit` struct for `chpst.c`. 767a977c Fixed function syntax in shell script. fbeaee71 Made inline functions static so they are included in the function. 5203b2a9 Updated patch to run the shell by default. f4893a38

1.3.1 - Fixed `Makefile` deprecated syntax and removed error on warnings from `Makefile.flags` from 1.3.0. Fixed newlines in config generation from 1.2.0. Merged `xatonum` patches from 1.3.0 (f815ab28 5203b2a9) into one to fix inline functions. 4fc47e74 Merged open file mode patches (3edf66cf 1.00-pre1, 23f4588e 1.1.1) into one. 99c8e894 Combined patches from 1.3.0 that dealt with `resource.h` for `rlimit`, `rusage`, and other identifiers (4e8b0943 9c02527c 57b84181 767a977c). 397b2dc4 Patched in system calls from 1.1.1. Use system-provided sysinfo from 1.3.0. Fixed conflicting `iphdr` from 1.2.0. Fix shell function syntax from 1.3.0. Run a shell by default from 1.3.0.

1.3.2 - Used updated `Makefile` and `Makefile.flags` from 1.3.0. Fixed newlines in config generation from 1.2.0. Fixed inline functions, open file mode, resource limits from 1.3.1. Fixed system calls from 1.1.1. Fixed sysinfo from 1.3.0. Fixed iphdr from 1.2.0. Fixed shell function syntax and run the shell by default from 1.3.0.

1.4.0 through 1.4.2 - Used updated `Makefile` and `Makefile.flags` from 1.3.0. Fixed newlines in config generation from 1.2.0. Fixed open file mode and resource limits from 1.3.1. Fixed system calls from 1.1.1. Fixed sysinfo from 1.3.0. Fixed iphdr from 1.2.0. Fixed shell function syntax and run the shell by default from 1.3.0.

1.5.0 - Used updated `Makefile` from 1.3.0. Updated resource limits patch. d17a98a8 Fixed sysinfo from 1.3.0. Fixed iphdr from 1.2.0. Fixed system calls from 1.1.1. Run shell by default from 1.3.0.

1.5.1 through 1.5.2 - Used updated `Makefile` from 1.3.0. Applied resource limits from 1.5.0. Fixed sysinfo from 1.3.0. Fixed iphdr from 1.2.0. Fixed system calls from 1.1.1. Run shell by default from 1.3.0.

1.6.0 - Used updated `Makefile` from 1.3.0. Updated resource limit patch. 93b05ab6 Updated sysinfo patch. d095b358 Updated iphdr patch. fcab7318 Fixed system calls from 1.1.1. Updated patch to run shell by default. 17061881

1.6.1 through 1.6.2 - Used updated `Makefile` from 1.3.0. Applied resource limit patch from 1.6.0. Applied sysinfo and iphdr patches from 1.6.0. Fixed system calls from 1.1.1. Applied change to run shell by default from 1.6.0.

1.7.0 - Used updated `Makefile` from 1.3.0. Applied resource limit patch from 1.6.0. Applied sysinfo patch from 1.6.0. Updated iphdr patch. 4715af4d Fixed conflicting network headers by defining a constant. 57719707 Fixed system calls from 1.1.1. Applied change to run shell by default from 1.6.0.

1.7.1 through 1.7.5 - Used updated `Makefile` from 1.3.0. Applied resource limit patch from 1.6.0. Applied sysinfo patch from 1.6.0. Applied iphdr and network header patches from 1.7.0. Fixed system calls from 1.1.1. Applied change to run shell by default from 1.6.0.

1.8.0 - Used updated `Makefile` from 1.3.0. Applied resource limit patch from 1.6.0. Applied sysinfo patch from 1.6.0. Applied iphdr and network header patches from 1.7.0. Fixed system calls from 1.1.1. Updated change to run shell by default. ce7f75f9

1.8.1 through 1.8.3 - Used updated `Makefile` from 1.3.0. Applied resource limit patch from 1.6.0. Applied sysinfo patch from 1.6.0. Applied iphdr and network header patches from 1.7.0. Fixed system calls from 1.1.1. Added change to run shell by default from 1.8.0.

1.9.0 - Used updated `Makefile` from 1.3.0. Applied network header patches from 1.7.0. Applied resource limit patch from 1.6.0 Updated sysinfo patch. 36515085 Applied iphdr patch from 1.7.0. Fixed system calls from 1.1.1. Updated patch to run the shell by default. 4fa45191

1.9.1 - Used updated `Makefile` from 1.3.0. Applied network header patches from 1.7.0. Applied resource limit patch from 1.6.0 Applied sysinfo patch from 1.9.0. Applied iphdr patch from 1.7.0. Fixed system calls from 1.1.1. Applied patch to run the shell by default from 1.9.0.

1.9.x is broken for ash (Segmentation fault) and lash (applet not found).
1.10.x is broken for lash (applet not found).

1.10.1 updated a patch

1.11.0 Included another patch to avoid gcc's `fcntl.h` and use the Linux one instead. Remove unnecessary inclusion of `sys/file.h`. Added `stime()` patch. Added `major()` and `minor()` patch.

1.11.1 Updated `fcntl.h` patch to include many more files. Updated patch to remove `sys/file.h` to eliminate redefinition of `flock64`. Added patch to stop building v2.4 kernel module tools.

1.12.x Updated patch to implement `stime()`.

1.11.0 through 1.13.4 -Typically use these patches: cb384d74 93b05ab6 5aabc4a3 009a632f 4715af4d 1303d9ed 3244c7b2

1.14.x - Used Makefile patch (cb384d74). Updated rlimit patch (c6dab8a1). New patch to build on JFFS2 (9807727b). 

1.15.x - Used Makefile patch (cb384d74). Used rlimit patch (53e69435). Updated major() patch (3f889f86). Used stime patch (3244c7b2).

1.16.0 - Used Makefile patch (cb384d74). Updated rlimit patch (b31ed008). Used major() patch (3f889f86). Used stime patch (3244c7b2).

1.16.1 through 1.16.2 - Used Makefile patch (cb384d74). Updated rlimit patch (b31ed008). Used major() patch (3f889f86). Used stime patch (3244c7b2). Added a patch to define `PRIO_PROCESS` and `setpriority` (5d09171a). Added a patch to update EXT2 for current includes (e71a71ba).

1.17.0 through 1.17.1 - Updated Makefile patch (91f46e17). Updated EXT2 patch (28126ee8). Added `PRIO_PROCESS` patch (5d09171a). Updated rlimit patch (5a02f3b9). Used major() patch (3f889f86). Used stime patch (3244c7b2).

1.17.2 through 1.17.4 - Updated EXT2 patch (28126ee8). Added `PRIO_PROCESS` patch (5d09171a). Updated rlimit patch (5a02f3b9). Used major() patch (3f889f86). Used stime patch (3244c7b2).

1.18.0 - Backported gen_build_files from 1.18.1 (91ce3536). Added EXT2 patch (28126ee8). Updated rlimit/rusage/PRIO_PROCESS patch (6d9a132b). Updated major/minor patch (32c7f767). Added stime patch (3244c7b2).

1.18.1 through 1.18.5 - Added EXT2 patch (28126ee8). Used limit/rusage/PRIO_PROCESS patch (6d9a132b). Included major/minor patch (32c7f767). Added stime patch (3244c7b2).

1.19.0 - Used limit/rusage/PRIO_PROCESS patch (6d9a132b). Added EXT2 patch (28126ee8). Added stime patch (3244c7b2).

1.19.1 - Used limit/rusage/PRIO_PROCESS patch (6d9a132b). Added EXT2 patch (28126ee8). Added stime patch (3244c7b2). Backported change from 1.19.2 to allow match_fstype to build (b09d9160)

1.19.2 through 1.19.4 - Used limit/rusage/PRIO_PROCESS patch (6d9a132b). Added EXT2 patch (28126ee8). Added stime patch (3244c7b2).

1.20.x - Used limit/rusage/PRIO_PROCESS patch (6d9a132b). Added stime patch (3244c7b2).

1.21.0 through 1.31.1 - Added stime patch (3244c7b2).

1.32.0 through 1.34.0 - No patches needed.
