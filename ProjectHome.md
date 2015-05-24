## Current Version: 0.6.3.2 ##

### Overview ###

Bocfel is an interpreter for the [Z-machine](http://en.wikipedia.org/wiki/Z-machine).  It fully supports versions 1-5, 7, and 8, and contains partial support for version 6.  For  detailed information on Bocfel's operation, please consult the [man page](http://bocfel.org/bocfel.html).

### The Z-machine ###
The Z-machine was designed to run text adventure games, also known as interactive fiction.  Originally the only Z-machine games were created by Infocom, the company that created the Z-machine.  These include such games as Zork, The Hitchhiker's Guide to the Galaxy, and Planetfall.  Fans of the genre figured out the format of the Z-machine, allowing non-Infocom interpreters, such as this one, to be built.

After that, a compiler for the Z-machine, called [Inform](http://www.inform-fiction.org/), was released.  Initially a language meant for programmers, the latest iteration of Inform is intended to allow non-programmers to easily write interactive fiction.  Thanks to Inform, hundreds of Z-machine story files have been written by enthusiasts, a number of which are of extremely high quality.

Although interactive fiction is today a rather niche genre, it has a loyal following of both players and authors, and can be explored through the following resources, among others:

  * [The Interactive Fiction Database](http://ifdb.tads.org/)
  * [IFWiki](http://www.ifwiki.org/)
  * [Baf's Guide to the IF Archive](http://www.wurb.com/if/)
  * [Annual Interactive Fiction Competition](http://www.ifcomp.org/)
  * [XYZZY Awards](http://xyzzyawards.org/)
  * [The Interactive Fiction Community Forum](http://www.intfiction.org/forum/)
  * The newsgroups rec.arts.int-fiction and rec.games.int-fiction

### Screenshots ###
[Beyond Zork](http://bocfel.org/screenshots/bd_curses.png) under [glktermw](http://www.eblong.com/zarf/glk/).

[The Mad Bomber](http://bocfel.org/screenshots/bomber_garglk.png) Z-machine abuse under [garglk](http://code.google.com/p/garglk/).

[TerpEtude](http://bocfel.org/screenshots/etude_none.png) running under the "dumb" interface which, despite its name, understands a bit about Unix terminals.

[Mingsheng](http://bocfel.org/screenshots/mingsheng_garglk.png) running under garglk, showing off Unicode support.

[Plundered Hearts](http://bocfel.org/screenshots/plundered_qglk.png) running under [QGlk](http://www.bubblycloud.com/qglk/).

[Spider and Web](http://bocfel.org/screenshots/tangler_garglk.png) Russian translation under garglk, also showing off Unicode.

[Zork](http://bocfel.org/screenshots/zork_winglk.png) running under [Windows Glk](http://www.ifarchive.org/indexes/if-archiveXprogrammingXglkXimplementations.html).

[The Dreamhold](http://bocfel.org/screenshots/dreamhold_nanoglk.png) running under [NanoGlk](http://www.ifarchive.org/indexes/if-archiveXprogrammingXglkXimplementations.html).

### Some of Bocfel's Features ###
  * Almost no platform-specific functions are used—and those that are used are optional—so almost any system with a recent C compiler should be able to build and run Bocfel.
  * Makes use of [Glk](http://eblong.com/zarf/glk/) for input/ouput, with complete support for [Gargoyle](http://garglk.googlecode.com/); a non-Glk “dumb” interface is also available.
  * Support (assuming a font with Unicode box-drawing characters) for the character graphics font used by Beyond Zork.
  * Unicode support: see, for example, Chinese characters used by [Mingsheng](http://ifdb.tads.org/viewgame?id=wjkg89918ttdbkm2) or the Russian translation of [Spider and Web](http://ifdb.tads.org/viewgame?id=2xyccw3pe0uovfad).
  * Multiple undo in almost all games, including those which do not natively support it.
  * Full control over command recording, transcripting, and command-record playback.
  * Rudimentary “cheating” support, designed to disable hunger and thirst daemons.

Only the source code to Bocfel is provided here.  If you are interested in a runnable binary, Ben Cressey has integrated Bocfel into the latest version of
[Gargoyle](http://garglk.googlecode.com/) as the default Z-machine interpreter.