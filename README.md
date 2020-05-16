# QED for Unix, UTF8/Unicode aware.

This is a port of Rob Pike's version of the QED editor for Unix, supporting
fully UTF8-encoded Unicode.

The port was developed on a modern Linux (Fedora 32). It
depends on just a few low-level kernel calls, so should be reasonably
portable accross any Unix-like OS (*BSD, MacOS).

The sources that this port began with were scavenged from Arnold Robbins's
[qed-archive](https://github.com/arnoldrobbins/qed-archive.git). Specifically
they are from the `unix-1992` sub-directory, which is from a tarball
of Rob Pike's original sources of the University of Toronto version of QED.

The manpage and tutorial in the `doc` subdirectory are essential (and fascinating) reading.

The `Makefile` provides a simple way to build a `qed` binary.

The more elaborate `mkfile` can build, install, and create a tarball.
It can also run off `pdf` versions of the turtorial and manpage. However, it
depends on you having a working [plan9port](https://github.com/9fans/plan9port).
