Tcsh
====

An improved C shell with command-line completion.

Git Source (6.06.01 and forward): https://github.com/tcsh-org/tcsh

Older Archives: http://ftp.lip6.fr/pub/unix/shells/tcsh/old/


Build Notes
-----------

6.00.00 - Removed `gcc` option -fcombine-regs. bfe0bf0 Included `time.h` to get the `tm` struct. 205594c Removed a check for `_SEQENT_`. 7586a71 Added `config/config.linux`, based on a later config. c2e34d6

6.00.01 - Added config, `gcc` option, and `_SEQENT_` fixes from 6.00.01. Recreated patch to include `time.h`. a6f0234

6.00.02 - Added config, `gcc` option, and `_SEQENT_` fixes from 6.00.01. Added time patch from 6.00.01.

6.00.02 - Added config from 6.00.01. Fixed `gcc` option patch. e044359 Updated the time patch. 47eb51d

6.01.00 - Added config from 6.00.01. Added `gcc` option and time patches from 6.00.02. Needed the crypt library. 264ddcc

6.02 - Fixed declarations of `gethostname` and `readlink`. 8f236d1 Updated the time patch. 031fa4b Fixed initialization of `sigset_t`. 900cad0 Added crypt library from 6.01.00.

6.03 - Added time patch from 6.02. Updated crypt library patch. a110fca

6.04 - Force Linux to not use a wait union. 8701288 Added time patch from 6.02. Updated crypt library patch. 0eefd91

6.05 - Included wait union change from 6.04. Added time patch from 6.02. Added crypt library patch from 6.03 because `Imakefile` now detects the crypt library.

6.06 - Removed inclusion of `localeinfo.h`. d5484e2 Updated wait union patch. 1649105 Added time patch from 6.02.

6.06.01 - Switched to the git repository. Added `config/linux` from 6.06. 2ab4536 Added wait union patch from 6.06. Removed unnecessary declaration of `crypt`. 5215340 Added time patch from 6.02.

6.06.02 - Reused `config/linux` patch from 6.06.01. Backported `config.guess` from 6.07.01. 257e5b4 Added wait union patch from 6.06. Adding time patch from 6.02. Added crypt library. f541b4b

6.06.03 through 6.07.00 - Used `config.guess` from 6.06.02. Used `config/linux` patch from 6.06.01. Added wait union patch from 6.06. Added time patch from 6.02. Added crypt library from 6.06.02.

6.07.01 through 6.07.04 - Used `config/linux` patch from 6.06.01. Added wait union patch from 6.06. Added time patch from 6.02.

6.07.05 - Removed declaration of `gethostname`. d287502 Added mode parameter to `open` call. 12180ec Fixed missing semicolon for RLIM_TYPE. 1fe32b4 Added wait union patch from 6.06. Added time patch from 6.02.

6.07.06 through 6.07.08 - Removed declaration of `gethostname` and added mode parameter to `open` call, both from 6.07.05. Added wait union patch from 6.06. Added time patch from 6.02.

6.07.09 - Added mode parameter to `open` call from 6.07.05. Added wait union patch from 6.06. Added time patch from 6.02.

6.07.10 - Added mode parameter to `open` call from 6.07.05. Fixed double semicolons. 91bd756 Added wait union patch from 6.06. Fixed F_DOSIFY_PREV. 1a4d777 Added time patch from 6.02.

6.07.11 through 6.08.04 - Added mode parameter to `open` call from 6.07.05. Added wait union patch from 6.06. Added time patch from 6.02.

6.08.05 - Add support for x86_64. 66ae601 Added mode parameter to `open` call from 6.07.05. Added wait union patch from 6.06. Added time patch from 6.02.

6.08.06 through 6.09.01 - Included x86_64 from 6.08.05. Added mode parameter to `open` call from 6.07.05. Added wait union patch from 6.06. Added time patch from 6.02.

6.09.02 - Included x86_64 from 6.08.05. Added mode parameter to `open` call from 6.07.05. Added wait union patch from 6.06. Fixed misplaced brace. 2a0ef73 Added time patch from 6.02.

6.09.03 - Included x86_64 from 6.08.05. Added mode parameter to `open` call from 6.07.05. Added wait union patch from 6.06. Added time patch from 6.02.

6.09.03 - Included x86_64 from 6.08.05. Updated mode parameter patch. 6c057e2. Added wait union patch from 6.06. Added time patch from 6.02.

6.10.00 - Included x86_64 from 6.08.05. Used mode parameter patch from 6.09.03. Added wait union patch from 6.06. Added time patch from 6.02.

6.10.01 - Updated x86_64 patch. b23e1b3 Used mode parameter patch from 6.09.03. Forced inclusion of GLOB constants. f4e8ea1

6.10.02 through 6.11.03 - Used x86_64 and GLOB patches from 6.10.01. Added wait union patch from 6.06.

6.11.04 - Used x86_64 patch from 6.10.01. Added wait union patch from 6.06.

6.11.05 through 6.13.05 - Added wait union patch from 6.06.

6.13.06 - Updated wait union patch. 9a4912b

6.13.07 - Used wait union patch from 6.13.06.

6.13.08 - Used wait union patch from 6.13.06. Corrected patchlevel.

6.13.09 through 6.14.02 - Used wait union patch from 6.13.06.

6.14.03 - Used wait union patch from 6.13.06. Fixed infinite loop. 5453b8c

6.14.04 through 6.14.05 - Used wait union patch from 6.13.06. Applied infinite loop fix from 6.14.03.

6.14.06 through 6.16.00 - Used wait union patch from 6.13.06.

6.16.01 through 6.17.02 - Used wait union patch from 6.13.06. Applied infinite loop fix from 6.14.03.

6.17.03 - Updated wait union patch. 4367bbb Applied infinite loop fix from 6.14.03.

6.17.04 through 6.17.07 - Used wait union patch from 6.17.03. Applied infinite loop fix from 6.14.03.

6.17.08 - Used wait union patch from 6.17.03. Fixed `malloc_usable_size` signature. d1902b0 Applied infinite loop fix from 6.14.03.

6.17.09 through 6.17.10 - Used wait union patch from 6.17.03. Applied infinite loop fix from 6.14.03.

6.18.00 - Used wait union patch from 6.17.03. Created new infinite loop fix - same symptoms. dd6153f

6.18.01 through 6.19.00 - Used wait union patch from 6.17.03. Used infinite loop fix from 6.18.00.

6.19.01 through 6.20.00 - Clean build.
