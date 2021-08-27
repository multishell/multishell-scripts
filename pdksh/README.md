`pdksh`
=======

Probably not worth it because I can't get any version to build correctly and have it work as expected.

Sources:

* 4.5 and 5.2.3: http://ftp.cc.uoc.gr/old/pub/shells/
* 5.0.6: http://ftp.is.co.za/mirror/ftp.slackware.com/pub/slackware-2.3/source/contrib/pdksh/
* 5.2.8: https://www.ibiblio.org/pub/Linux/system/shells/
* 5.2.12, 5.2.13, 5.2.14: http://ftp.lip6.fr/pub/unix/shells/pdksh/


Build Notes
-----------

4.5 - Commented out conflicting definitions (69cf48d).

5.0.6 - Fixed `errno` in a struct because it's also defined as a macro (c1736ea). Fixed signal generation script to work with multiline defined signals (c0d73c7).

5.2.3 - Fixed quoting issue in configure script (7701de2). Used signal generation script (c0d73c7).

5.2.8 - Used configure script patch (7701de2). Used signal generation script (c0d73c7).

5.2.12 - Updated signal generation script (d20fc08). Can not get the build to work - I'm not good at m4.

5.2.13 - Can not get the build to work - I'm not good at m4.

5.2.14 - Used signal patch (d20fc08). Can not get the build to work - I'm not good at m4.
