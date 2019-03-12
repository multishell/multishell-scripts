Apple's Bash
============

Apple shipped Bash 2.x early on, then switched to Bash 3.x, but did not proceed to Bash 4.x over licensing concerns.

The source to Bash is either within a `bash` or a `bash-3.2` folder.

Source:  https://opensource.apple.com/tarballs/bash/

`strlcat` source: http://ftp3.usa.openbsd.org/pub/OpenBSD/src/lib/libc/string/strlcat.c and strlcat.h


Building Notes
--------------

23 - Parallel build is broken. Patched in support for AMD64.

25 - Parallel build is broken. Patched the "label at end of compound statement" fix. `41a9993`

29 through 44.3 - Parallel build is broken. Cherry picked "label at end of compound statement" fix from 25.

44.4 through 44.5 - Parallel build is broken. Cherry picked "label at end of compound statement" fix from 25. Conditionally include `signal.h` in `lib/readline/display.c`. `d4ba95e`

76.1 - Parallel builds work. Removed detection of unsupported `EBADEXEC`. `ce4f10a`

76.2 through 80 - Cherry picked removal of `EBADEXEC` from 76.1.

84 - Cherry picked removal of `EBADEXEC` from 76.1. `make` automatically ran `configure`. First version where directory name is `bash-3.2`.

84.1.2 - Cherry picked removal of `EBADEXEC` from 76.1. Needed to add `strlcat`. 9d69109

86.1 - Cherry picked removal of `EBADEXEC` from 76.1.

86.1.2 - Cherry picked removal of `EBADEXEC` from 76.1 and `strlcat` from 84.1.2.

92 - Cherry picked removal of `EBADEXEC` from 76.1.

92.1.2 through 94.1.2 - Cherry picked removal of `EBADEXEC` from 76.1 and `strlcat` from 84.1.2.

97 through 106.201.1 - Cherry picked removal of `EBADEXEC` from 76.1.

106.220.2 - Identical to 106.201.1. Cherry picked removal of `EBADEXEC` from 76.1.

Fixing errors:
 * `EBADEXEC` - cherry-pick `ce4f10a` from 76.1
 * `strlcat` - cherry-pick `9d69109` from 84.1.2
