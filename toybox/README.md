Toybox
======

Alternative to Busybox; a single executable that bundles together many common Linux command-line utilities.

Source: http://www.landley.net/toybox/downloads/


Build Notes
-----------

0.0.1 - Built fine.

0.0.2 - Patched kconfig/Makefile to expand braces for portability (856babd). Commented out `inline` to allow function to be linked and found for kconfig (f58e6bb).

0.0.3 through 0.0.4 - Commented out `inline` to allow function to be linked and found for kconfig (f58e6bb).

0.0.5 through 0.1.0 - Commented out `inline` to allow function to be linked and found for kconfig (f58e6bb). Adding makedev macro (70a8332).

0.2.0 - Added patch from 0.0.2 to inline for kconfig (f58e6bb). Updated makedev macro (3288c0b). Added new patch for PRIO_PROCESS (4093051). Added new patch for major() and minor() (436f9a7).

0.2.1 through 0.3.0 - Added inline patch from 0.0.2 to inline for kconfig (f58e6bb). Adding makedev macro (3288c0b). Included PRIO_PROCESS (4093051). Added major() and minor() (436f9a7)/

0.3.1 - Added patch from 0.0.2 to inline for kconfig (f58e6bb). Added new patch to fix the number of arguments to dirtree_read (5927c3b). Recreated patch for major() and minor() (2fd596f). Updated makedev macro (9fc317b).

0.4.0 - Added patch from 0.0.2 to inline for kconfig (f58e6bb). Included major()/minor() patch (2fd596f). Included makedev macro (9fc317b). Updated dirtree_read patch (f44919c).

0.4.1 - Added patch from 0.0.2 to inline for kconfig (f58e6bb). Included major()/minor() patch (2fd596f). Updated makedev macro (8eba680). Added dirtree_read patch (f44919c).
