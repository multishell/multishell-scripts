Bash
====

One of the most pervasive shells for Unix-style systems.

Source: https://ftp.gnu.org/gnu/bash/


Build Notes
-----------

1.14.7 - Does not compile.

2.0 - Compiles, core dump.

2.02 - First version that compiles and runs.

2.05a - Rewrote configure and Makefile.  Broke parallel make.

3.00.0 - Bulk builder works from here on.  Probably works on 2.02 and forward.

3.00.23 - Needed to rebuild `y.tab.c` and `y.tab.h` because committed versions were behind `parse.y`. `touch parse.y && make`.

3.2.38 - Needed to rebuild `y.tab.c` and `y.tab.h` because committed versions were behind `parse.y. `touch parse.y && make`.
