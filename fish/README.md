Fish
====

Source: https://fishshell.com/


Build Notes
-----------

1.16.0 - Using the internal version of wcsncasecmp because the system-provided version has a fourth parameter. 63e9758 Also had to use a file mode with `__open_missing_mode ()`. fe24042

1.16.1 - `wcsncasecmp` patch updated because it did not cherry pick cleanly. 02018c3 Applied `__open_missing_mode ()` fix from 1.16.0.

1.16.2 - Applied `wcsncasecmp` from 1.16.1 and `__open_missing_mode ()` from 1.16.0.

1.17.0 - Updated `wcsncasecmp` patch to handle a conflict. b486db8 Applied `__open_missing_mode ()` from 1.16.0.

1.18.0 through 1.18.1 - Applied `wcsncasecmp` from 1.17.0 and `__open_missing_mode ()` from 1.16.0.

1.19.0 - Applied `__open_missing_mode ()` from 1.16.0. `wcsncasecmp` patch changed again and the auto-detection does not check the number of parameters, so made a patch to still use the internal version. 0541d92

1.20.0 - `wcsncasecmp` patch changed again. d60497f Applied `__open_missing_mode ()` from 1.16.0. Had to correct version number from 1.19.0.

1.20.1 - `wcsncasecmp` did not apply cleanly, updated. 093cf74 Applied `__open_missing_mode ()` from 1.16.0. Had to correct version number from 1.19.0. Removed `fish_pager.txt` from `Makefile.in` because it did not exist. d7f7385

1.20.2 - Applied `wcsncasecmp` from 1.20.1 and `__open_missing_mode ()` from 1.16.0. The `fish_pager.txt` patch changed. c4a37df

1.21.0 - Applied `wcsncasecmp` from 1.20.1 and `__open_missing_mode ()` from 1.16.0.

1.21.2 - Updated `wcsncasecmp` patch. 32c64f2 Applied `__open_missing_mode ()` from 1.16.0. Fixed a missing `wint_t` type.

1.21.3 through 1.21.9 - Applied `__open_missing_mode ()` from 1.16.0.

1.21.10 - Applied `__open_missing_mode ()` from 1.16.0. Found issue building `builtin_help.c`.

1.21.11 through 1.22.3 - Applied `__open_missing_mode ()` from 1.16.0. Found issue building `builtin_help.c`.

1.23.0 - Removed whitespace in `configure.ac` that caused errors. Include `linux/limits.h` to define ARG_MAX.

1.23.1 - Fixed version number in `configure.ac`.

2.5b1 - First build that looks for a `version` file.
