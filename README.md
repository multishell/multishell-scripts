Multishell
==========

This repository contains the build scripts and tools that are necessary to build the [Multishell Docker Image](https://hub.docker.com/r/fidian/multishell/).


Version Numbers
---------------

I've attempted to publish as many versions of the shells as I was able to find. Each version is represented as a branch in the git repository, with a tag pointing to the files as they were retrieved from their original source. Any later commits to that branch were done to aid in compilation.

The `all-versions` file lists every version that would compile. It corresponds to tag names, and you can prefix the version with `ms_` to get the branch name. They do not represent the final version number and possibly not the command that's built. In some cases, such as with Bash, the branch might be "4.0" but the final version number is "4.0.0". In other cases, such as with Apple's version of Bash, the branch name is their internal version number and that does correspond to the built binary, but the `apple-bash-92` program will report "Bash version 3.2.51(2)" as its version number.

Sorry for the confusion. Here's a few examples.

| Shell      | Tag      | Branch      | Command             | Internal version   |
|------------|----------|-------------|---------------------|--------------------|
| Bash       | 3.0.12   | ms_3.0.12   | bash-3.00.12        | 3.00.12(2)-release |
| Bash       | 3.2      | ms_3.2      | bash-3.2.0          | 3.2.0(2)-release   |
| Bash       | 4.4.1    | ms_4.4.1    | bash-4.4.1          | 4.4.1(1)-release   |
| Apple Bash | 97       | ms_97       | apple-bash-97       | 3.2.57(2)-release  |
| Apple Bash | 103.50.1 | ms_103.50.1 | apple-bash-103.50.1 | 3.2.57(2)-release  |

* Shell: The name of the type of shell that was compiled.
* Tag: The tag name in our version of the source repository for the original source before any necessary modifications were made.
* Branch: The branch name in our version of the source repository. This contains additional commits in order to make the source code compile.
* Command: The executable's name when it is installed to `/usr/local/bin/`.
* Internal version: What the shell reports as its version. Apple's Bash is especially unhelpful in this regard.

In addition to the many executables, there's symlinks to get the most recent version of a particular release. So, running `bash-3.2` would actually run `bash-3.2.57`.
