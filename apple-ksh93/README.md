Apple's Ksh93
=============

Apple's version of AT&T's Korn shell.

Source: https://opensource.apple.com/tarballs/ksh/


Build Notes
-----------

4 - Allowing the build to work on newer versions of Linux with regard to `ast.h`. `b2ce7b3` Fixing `iffe.sh` and the detection of library functions. `1bd753f` Correcting value for `L_tmpnam`. `b90eebd` Added earlier termination and easier problem detection to `mamake`. `91afa48` Use internal versions of `major()`, `minor()`, and `makedev()`. `6445b2c`

13 - Corrected defined variable names for endianness. `2e3e2cd` Updated patch to get the build to work on newer versions of Linux. `064d7fd` Updated `L_tmpnam` patch. `be2db2b` Applied `mamake` termination patch from 4. Use internal major/minor/makedev from 4.

16.1 - Used patch for newer versions of Linux from 4. Used `L_tmpnam` patch from 13. `be2db2b` Applied `mamake` termination patch from 4. Use internal major/minor/makedev from 4.

18 - Updated endianness patch. `b1db1e6` Updated patch for newer versions of Linux for `ast.h`. `948e565` Used `L_tmpnam` patch from 13. Applied `mamake` termination patch from 4. Use internal major/minor/makedev from 4.

20 - Added endianness from 18. Added compilation on Linux from 18. Used `L_tmpnam` patch from 13. Applied `mamake` termination patch from 4. Use internal major/minor/makedev from 4.

23 through 28 - Applied `mamake` termination patch from 4. Added endianness from 18. Added compilation on Linux from 18. Used `L_tmpnam` patch from 13. Use internal major/minor/makedev from 4.

* `mamake` termination patch from 4 `91afa48`
* Endianness from 18 `b1db1e6`
* ast.h Compilation on Linux from 18 `948e565`
* `L_tmpnam` from 13 be2db2b
* Internal major/minor/makedev from 4 `6445b2c`
