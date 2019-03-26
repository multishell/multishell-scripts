Multishell
==========

This repository contains the build scripts and tools that are necessary to build the [Multishell Docker Image](https://hub.docker.com/r/fidian/multishell/).


Available Versions
------------------

* apple-bash
    * 23, 25, 29, 30, 44.2, 44.3, 44.4, 44.5, 76.1, 76.2, 80, 84, 84.1.2, 86.1, 86.1.2, 92, 92.1.2, 94.1.2, 97, 99, 103, 103.50.1, 106, 106.201.1, 106.220.2
* apple-ksh93
    * 4, 13, 16.1, 18, 20, 23, 25
* bash
    * 2.x series
        * 2.02.0, 2.02.1, 2.03.0, 2.04.0, 2.05a.0, 2.05b.0, 2.05.0
    * 3.00.x series
        * 3.00.0, 3.00.1, 3.00.2, 3.00.10, 3.00.11, 3.00.12, 3.00.13, 3.00.14, 3.00.15, 3.00.16, 3.00.17, 3.00.18, 3.00.19, 3.00.20, 3.00.21, 3.00.22, 3.00.23
    * 3.1.x series
        * 3.1.0, 3.1.1, 3.1.2, 3.1.3, 3.1.4, 3.1.5, 3.1.6, 3.1.7, 3.1.8, 3.1.9, 3.1.10, 3.1.11, 3.1.12, 3.1.13, 3.1.14, 3.1.15, 3.1.16, 3.1.17, 3.1.18, 3.1.19, 3.1.20, 3.1.21, 3.1.22, 3.1.23
    * 3.2.x series
        * 3.2.0, 3.2.1, 3.2.2, 3.2.3, 3.2.4, 3.2.5, 3.2.6, 3.2.7, 3.2.8, 3.2.9, 3.2.10, 3.2.11, 3.2.12, 3.2.13, 3.2.14, 3.2.15, 3.2.16, 3.2.17, 3.2.18, 3.2.19, 3.2.20, 3.2.21, 3.2.22, 3.2.23, 3.2.24, 3.2.25, 3.2.26, 3.2.27, 3.2.28, 3.2.29, 3.2.30, 3.2.31, 3.2.32, 3.2.33, 3.2.34, 3.2.35, 3.2.36, 3.2.37, 3.2.38, 3.2.39, 3.2.40, 3.2.41, 3.2.42, 3.2.43, 3.2.44, 3.2.45, 3.2.46, 3.2.47, 3.2.48, 3.2.49, 3.2.50, 3.2.51, 3.2.52, 3.2.53, 3.2.54, 3.2.55, 3.2.56, 3.2.57
    * 4.0.x series
        * 4.0.0, 4.0.0-rc1, 4.0.1, 4.0.2, 4.0.3, 4.0.4, 4.0.5, 4.0.6, 4.0.7, 4.0.8, 4.0.9, 4.0.10, 4.0.11, 4.0.12, 4.0.13, 4.0.14, 4.0.15, 4.0.16, 4.0.17, 4.0.18, 4.0.19, 4.0.20, 4.0.21, 4.0.22, 4.0.23, 4.0.24, 4.0.25, 4.0.26, 4.0.27, 4.0.28, 4.0.29, 4.0.30, 4.0.31, 4.0.32, 4.0.33, 4.0.34, 4.0.35, 4.0.36, 4.0.37, 4.0.38, 4.0.39, 4.0.40, 4.0.41, 4.0.42, 4.0.43, 4.0.44
    * 4.1.x series
        * 4.1.0, 4.1.1, 4.1.2, 4.1.3, 4.1.4, 4.1.5, 4.1.6, 4.1.7, 4.1.8, 4.1.9, 4.1.10, 4.1.11, 4.1.12, 4.1.13, 4.1.14, 4.1.15, 4.1.16, 4.1.17
    * 4.2.x series
        * 4.2.0, 4.2.1, 4.2.2, 4.2.3, 4.2.4, 4.2.5, 4.2.6, 4.2.7, 4.2.8, 4.2.9, 4.2.10, 4.2.11, 4.2.12, 4.2.13, 4.2.14, 4.2.15, 4.2.16, 4.2.17, 4.2.18, 4.2.19, 4.2.20, 4.2.21, 4.2.22, 4.2.23, 4.2.24, 4.2.25, 4.2.26, 4.2.27, 4.2.28, 4.2.29, 4.2.30, 4.2.31, 4.2.32, 4.2.33, 4.2.34, 4.2.35, 4.2.36, 4.2.37, 4.2.38, 4.2.39, 4.2.40, 4.2.41, 4.2.42, 4.2.43, 4.2.44, 4.2.45, 4.2.46, 4.2.47, 4.2.48, 4.2.49, 4.2.50, 4.2.51, 4.2.52, 4.2.53
    * 4.3.x series
        * 4.3.0, 4.3.1, 4.3.2, 4.3.3, 4.3.4, 4.3.5, 4.3.6, 4.3.7, 4.3.8, 4.3.9, 4.3.10, 4.3.11, 4.3.12, 4.3.13, 4.3.14, 4.3.15, 4.3.16, 4.3.17, 4.3.18, 4.3.19, 4.3.20, 4.3.21, 4.3.22, 4.3.23, 4.3.24, 4.3.25, 4.3.26, 4.3.27, 4.3.28, 4.3.29, 4.3.30, 4.3.31, 4.3.32, 4.3.33, 4.3.34, 4.3.35, 4.3.36, 4.3.37, 4.3.38, 4.3.39, 4.3.40, 4.3.41, 4.3.42, 4.3.43, 4.3.44, 4.3.45, 4.3.46, 4.3.47, 4.3.48
    * 4.4.x series
        * 4.4.0, 4.4.0-beta, 4.4.0-beta2, 4.4.0-rc1, 4.4.0-rc2, 4.4.1, 4.4.2, 4.4.3, 4.4.4, 4.4.5, 4.4.6, 4.4.7, 4.4.8, 4.4.9, 4.4.10, 4.4.11, 4.4.12, 4.4.13, 4.4.14, 4.4.15, 4.4.16, 4.4.17, 4.4.18, 4.4.19, 4.4.20, 4.4.21, 4.4.22, 4.4.23
    * 5.0.x series
        * 5.0.0, 5.0.0-alpha, 5.0.0-beta, 5.0.0-beta2, 5.0.0-rc1, 5.0.1, 5.0.2
* dash
    * 0.5.2, 0.5.3, 0.5.4, 0.5.5, 0.5.5.1, 0.5.6, 0.5.6.1, 0.5.7, 0.5.8, 0.5.9, 0.5.9.1, 0.5.10, 0.5.10.1, 0.5.10.2
* fish
    * 1.x series
        * 1.16.0, 1.16.1, 1.16.2, 1.17.0, 1.18.0, 1.18.1, 1.19.0, 1.20.0, 1.20.1, 1.20.2, 1.21.0, 1.21.2, 1.21.3, 1.21.4, 1.21.5, 1.21.6, 1.21.7, 1.21.8, 1.21.9, 1.21.10, 1.21.11, 1.21.12, 1.22.0, 1.22.1, 1.22.3, 1.23.0, 1.23.1
    * 2.x series
        * 2.0.0, 2.1.0, 2.1.1, 2.1.2, 2.2b1, 2.2.0, 2.3b1, 2.3b2, 2.3.0, 2.3.1, 2.4b1, 2.4.0, 2.5b1, 2.5.0, 2.6b1, 2.6.0, 2.7b1, 2.7.0, 2.7.1
    * 3.x series
        * 3.0b1, 3.0.0, 3.0.1, 3.0.2
* sash
    * 3.4, 3.4-fmb, 3.5, 3.5-fmb, 3.6, 3.6-fb, 3.7, 3.7-fb, 3.8
* tcsh
    * 6.00.00, 6.00.01, 6.00.02, 6.00.03, 6.01.00, 6.02.00, 6.03.00, 6.04.00, 6.05.00, 6.06.00, 6.06.01, 6.06.02, 6.06.03, 6.06.04, 6.07.00, 6.07.01, 6.07.02, 6.07.03, 6.07.04, 6.07.05, 6.07.06, 6.07.07, 6.07.08, 6.07.09, 6.07.10, 6.07.12, 6.07.13, 6.08.00, 6.08.01, 6.08.02, 6.08.03, 6.08.04, 6.08.05, 6.08.06, 6.08.07, 6.09.00, 6.09.01, 6.09.02, 6.09.03, 6.09.04, 6.10.00, 6.10.01, 6.10.02, 6.11.00, 6.11.01, 6.11.03, 6.11.04, 6.11.05, 6.12.00, 6.12.01, 6.12.02, 6.12.03, 6.13.00, 6.13.01, 6.13.02, 6.13.03, 6.13.04, 6.13.05, 6.13.06, 6.13.07, 6.13.08, 6.13.09, 6.13.10, 6.14.00, 6.14.01, 6.14.02, 6.14.03, 6.14.04, 6.14.05, 6.14.06, 6.14.07, 6.15.00, 6.15.01, 6.15.02, 6.16.00, 6.16.01, 6.17.00, 6.17.01, 6.17.02, 6.17.03, 6.17.04, 6.17.05, 6.17.06, 6.17.07, 6.17.08, 6.17.09, 6.17.10, 6.18.00, 6.18.01, 6.18.02, 6.18.03, 6.18.04, 6.18.05, 6.19.00, 6.19.01, 6.20.00
* zsh
    * 3.x series
        * 3.0.8, 3.1.7, 3.1.8, 3.1.9
    * 4.x series
        * 4.0.1, 4.0.2, 4.0.4, 4.0.6, 4.0.7, 4.0.9, 4.2.0, 4.2.1, 4.2.3, 4.2.4, 4.2.5, 4.2.6, 4.2.7
    * 5.x series
        * 5.0.0, 5.0.1, 5.0.2, 5.0.4, 5.0.5, 5.0.6, 5.0.7, 5.0.8, 5.1, 5.1.1, 5.2, 5.3, 5.3.1, 5.4.1, 5.4.2, 5.5, 5.5.1, 5.6, 5.6.1, 5.6.2, 5.7, 5.7.1


Version Numbers
---------------

I've attempted to publish as many versions of the shells as I was able to find. Each version is represented as a branch in the git repository, with a tag pointing to the files as they were retrieved from their original source. Any later commits to that branch were done to aid in compilation.

The `all-versions` file lists every version that would compile. It corresponds to tag names, and you can prefix the version with `ms_` to get the branch name. They do not represent the final version number and possibly not the command that's built. In some cases, such as with Bash, the branch might be "4.0" but the final version number is "4.0.0". In other cases, such as with Apple's version of Bash, the branch name is their internal version number and that does correspond to the built binary, but the `apple-bash-92` program will report "Bash version 3.2.51(2)" as its version number.

Sorry for the confusion. Here's a few examples.

| Shell               | Tag      | Branch      | Command             | Internal version   |
|---------------------|----------|-------------|---------------------|--------------------|
| Apple Bash          | 103.50.1 | ms_103.50.1 | apple-bash-103.50.1 | 3.2.57(2)-release  |
| Apple Bash          | 97       | ms_97       | apple-bash-97       | 3.2.57(2)-release  |
| Bash                | 3.0.12   | ms_3.0.12   | bash-3.00.12        | 3.00.12(2)-release |
| Bash                | 3.2      | ms_3.2      | bash-3.2.0          | 3.2.0(2)-release   |
| Bash                | 4.4.1    | ms_4.4.1    | bash-4.4.1          | 4.4.1(1)-release   |
| Dash                | 0.5.6.1  | ms_0.5.6.1  | dash-0.5.6.1        | *none*             |
| Fish                | 2.7.0    | ms_2.7.0    | fish-2.7.0          | 2.7.0              |
| Fish                | 2.7b1    | ms_2.7b1    | fish-2.7b1          | 2.7b1              |
| Sash                | 3.7      | ms_3.7      | sash-3.7            | 3.7                |
| Sash (plus patches) | 3.7-fmb  | ms_3.7-fmb  | sash-3.7-fmb        | 3.7-fmb            |
| Tcsh                | 6.06     | ms_6.06     | tcsh-6.06.00        | 6.06.00            |
| Tcsh                | 6.20.00  | ms_6.20.00  | tcsh-6.20.00        | 6.20.00            |
| Zsh                 | 5.3      | ms_5.3      | zsh-5.3             | 5.3                |
| Zsh                 | 5.3.1    | ms_5.3.1    | zsh-5.3.1           | 5.3.1              |

* Shell: The name of the type of shell that was compiled.
* Tag: The tag name in our version of the source repository for the original source before any necessary modifications were made. This version number matches the version number of the source distribution.
* Branch: The branch name in our version of the source repository. This contains additional commits in order to make the source code compile. This version number matches the version number of the source distribution.
* Command: The executable's name when it is installed to `/usr/local/bin/`. This version number can be different and matches the internal version where applicable. Notibaly, you can see this more with Apple's Bash and some of the Bash releases, such as "3.2" in the above list.
* Internal version: What the shell reports as its version. Dash doesn't seem to have this set anywhere. Apple's Bash is especially unhelpful because it reports a version but you can't really use it for determining what version of Bash is running.

In addition to the many executables, there's symlinks to get the most recent version of a particular release. So, running `bash-3.2` would actually run `bash-3.2.57`.

**Apple Bash:** This has a funky versioning scheme, so use the full version number there when you care about which one you get. You can't run the shell and get the version number because it often reports `3.2.57(2)`. The symbolic links are created, but are essentially useless.

**Dash:** There's no way to double-check the version number of the binary beyond feature/bug detection.

**Tcsh:** I used tar files for the early releases and git tags for later versions, which is why the version number scheme differs.

**Zsh:** The symbolic links don't work well because the version number doesn't include the patch level if it's zero. Thus, running `zsh-5.6` will not run the newest in the 5.6.x series. Instead, you must specify the version number yourself; `zsh-5.6.2`, `zsh-5.6.1`, and `zsh-5.6` are all different commands. The symlink will exist for `zsh-5`, which would run the newest in the 5.x series.


Changes To The Shells
---------------------

Most builds needed changes in order to work within the Docker container. The patches are aimed to be as minimal as possible. All of the source repositories are [hosted on GitHub](https://github.com/multishell).
