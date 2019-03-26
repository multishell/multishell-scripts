Apple's Ksh93
=============

Apple's version of AT&T's Korn shell.

Source: https://opensource.apple.com/tarballs/ksh/


Build Notes
-----------

4 - Allowing the build to work on newer versions of Linux. b2ce7b3 Fixing `iffe.sh` and the detection of library functions. 1bd753f Correcting value for `L_tmpnam`. b90eebd Added earlier termination and easier problem detection to `mamake`. 91afa48

13 - Corrected defined variable names for endianness. 2e3e2cd Updated patch to get the build to work on newer versions of Linux. 064d7fd Updated `L_tmpnam` patch. be2db2b Applied `mamake` termination patch from 4.

16.1 - Used patch for newer versions of Linux from 4. Used `L_tmpnam` patch from 13. be2db2b Applied `mamake` termination patch from 4.

18 - Updated endianness patch. b1db1e6 Updated patch for newer versions of Linux. 948e565 Used `L_tmpnam` patch from 13. Applied `mamake` termination patch from 4.

20 - Added endianness from 18. Added compilation on Linux from 18. Used `L_tmpnam` patch from 13. Applied `mamake` termination patch from 4.

23 - Doesn't build `ast.h`. No errors seem to be reported to indicate why. Internally, version is 2012-08-01. Applied `mamake` termination patch from 4.

25 - Doesn't build `ast.h`. No errors seem to be reported to indicate why. Internally, version is 2012-08-01. Applied `mamake` termination patch from 4.
