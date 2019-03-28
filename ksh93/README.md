Ksh93
=====

AT&T's Korn shell.

Source: https://src.fedoraproject.org/lookaside/pkgs/rpms/ksh/


Build Notes
-----------

First, extract `INIT.*.tgz` into the folder. Copy in the `ast-ksh.*.tgz` archive. Run `bin/package read` to extract the package. Remove `ast-ksh.*.tgz` to clean up and commit everything as the first commit in a new branch.

2002-06-28 - Patched to let it compile on a newer version of Linux. ab680826 Fixing `iffe.sh` and the detection of library functions. e4ad3845 Used a function as `extern` to correct a `static` issue. 8b54af7a Fixing `L_tmpnam` being defined with no value. b41eceb9 Made `mamake` die from any eventual error much sooner and report a standard "error:" message. cf684659 Backported `src/cmd/INIT/LICENSE` from 2004-02-29 so `mamake` can compile. 344b054f

2004-02-29 - Added patch to let it compile on newer Linux systems from 2002-06-28. Updated `L_tmpnam` patch. fabf9658 Added `iife.sh` from 2002-06-28. Updated `mamake` patch. 834929bd

2004-12-25 - Added patch to let it compile on newer Linux systems from 2002-06-28. Added `L_tmpnam` patch from 2004-02-29. Updated patch to fix `static` issue with `extern`. cc09b4a5 Updated `iife.sh` patch. 5c4ee3fe Added `mamake` patch from 2004-02-29.

2005-02-02 - Added patch to let it compile on newer Linux systems from 2002-06-28. Added `L_tmpnam` patch from 2004-02-29. Added `static` vs `extern` from 2004-12-25. Added `mamake` patch from 2004-02-29.

2006-01-24 through 2006-02-14 - Added patch to let it compile on newer Linux systems from 2002-06-28. Added `L_tmpnam` patch from 2004-02-29. Added `mamake` patch from 2004-02-29.

2007-01-11 - Updated patch for newer Linux systems. 19b9d22e Updated `L_tmpnam` patch. aa780d93 Added `mamake` patch from 2002-06-28. Added `mamake` patch from 2004-02-29.

2007-03-28 through 2010-08-11 - Added patch to let it compile on newer Linux systems and `L_tmpnam` patch from 2007-01-11. Added `mamake` patch from 2004-02-29.

2010-08-26 - This problem build needs to have `bin/package make` ran multiple times. Added patch to let it compile on newer Linux systems and `L_tmpnam` patch from 2007-01-11. Added `mamake` patch from 2004-02-29.

2010-09-24 through 2011-01-18 - Added patch to let it compile on newer Linux systems and `L_tmpnam` patch from 2007-01-11. Added `mamake` patch from 2004-02-29.

2011-01-27 - Added patch to let it compile on newer Linux systems and `L_tmpnam` patch from 2007-01-11. Fixed "mamake [lib/libast]: don't know how to make features/sfio" by using a file from 2010-09-24. 502ec438 Added `mamake` patch from 2004-02-29.

2011-01-31 - Added patch to let it compile on newer Linux systems and `L_tmpnam` patch from 2007-01-11. Added `mamake` patch from 2004-02-29.

2011-02-02 through 2012-02-29 - Added `mamake` patch from 2004-02-29. Added patch to let it compile on newer Linux systems and `L_tmpnam` patch from 2007-01-11.

2012-05-18 - Added `mamake` patch from 2004-02-29. Added patch to let it compile on newer Linux systems and `L_tmpnam` patch from 2007-01-11. Backported all `Mamfile` from 2012-05-31 because these have many errors. 61f660a7 Restored previous `isoc99` and removed `asometh` features. 30dac196

2012-05-31 through 2012-08-01 - Added `mamake` patch from 2004-02-29. Added patch to let it compile on newer Linux systems and `L_tmpnam` patch from 2007-01-11.
