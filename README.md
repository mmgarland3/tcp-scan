# tcp-scan

This is a fork of the long-stagnant tcp-scan application.  My primary objective in forking this project was initially to update tcp-scan-services with new applications and services.
This is intended as a pentesting resource, but will also probably be useful for network and systems admins.

The TCP scanner.

Installation
------------

tcp-scan uses the standard GNU automake and autoconf tools, so the typical installation process is:

- Run ```git clone https://github.com/royhills/tcp-scan.git``` to obtain the project source code
- Run ```cd tcp-scan``` to enter source directory
- Run ```autoreconf --install``` to generate a viable ./configure file
- Run ```./configure``` to generate a makefile for your system
- Run ```make``` to build the project
- Optionally run ```make check``` to verify that everything works as expected
- Run ```make install``` to install (you'll need root or sudo for this part)

You will need GNU automake and autoconf, the make utility, an ANSI C compiler (for example gcc or clang), and the development header files and libraries.

You can pass various options to "configure" to control the build and
installation process.  See the file INSTALL for more details.

tcp-scan is known to compile and run on the following platforms:

 - Linux

The IP packets are sent using raw sockets, and the responses are received
using libpcap (http://www.tcpdump.org/).

Documentation
-------------

For usage information, including details of all the options, use:

```tcp-scan --help```

