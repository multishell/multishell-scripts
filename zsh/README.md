Zsh
===

Source: https://sourceforge.net/projects/zsh/files/zsh/


Build Notes
-----------

3.0.8 - Renamed `getline` to `getline_zsh` to not conflict with a library. 2188971

3.1.7 through 4.0.9 - Updated `getline` patch. 382dce3 Occasional flaky builds where SIGCOUNT was not defined because `signames.c` was empty. Suspect it's from building `signames.o` in parallel, so updated build script to build that sequentially before the parallel build.

4.2.0 - `getline` patch no longer needed.
