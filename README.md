# macOS-command-line

## System

### Package Manager

* [Homebrew](https://brew.sh/)

### Power

* _pmset_
```
	pmset sleepnow
``` 

### Network

* [networksetup](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man8/networksetup.8.html) configuration tool for network settings in System Preferences.

### File System

* _mdfind_
* [find](skills/find.md)
* _mount_
```
	# mount smbfs as a local volume.
	sudo mkdir /Volumes/Public
	sudo chown $(whoami) /Volumes/Public
	mount_smbfs smb://username@192.168.1.2/Public /Volumes/Public
```

## Image

* [sips](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/sips.1.html) scriptable image processing system.This tool is used to query or modify raster image files and ColorSync ICC profiles.  Its functionality can also be used through the "Image Events" AppleScript suite.
* [exiv2](http://www.exiv2.org/) Manage image metadata. It provides fast and easy read and write access to the Exif, IPTC and XMP metadata of digital images in various formats
* [exiftool](https://sourceforge.net/projects/exiftool/) Perl library and command-line application for reading, writing and editing meta information (EXIF, IPTC, XMP, and more) in a wide variety of file formats (JPEG, TIFF, PNG, PDF, RAW, and more).
* [pngquant](https://pngquant.org) pngquant is a command-line utility and a library for lossy compression of PNG images. The conversion reduces file sizes significantly (often as much as 70%) and preserves full alpha transparency. Generated images are compatible with all modern web browsers, and have better fallback in IE6 than 24-bit PNGs.

## Sound

* [afconvert](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/afconvert.1.html) Audio File Convert will convert a source audio file to a new audio file with the specified file and data types.
* [afplay](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/afplay.1.html) Audio File Play plays an audio file to the default audio output.
* [afinfo](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/afinfo.1.html) Audio File Info prints out information about an audio file to stdout

## Text

* [pandoc](http://pandoc.org/) Pandoc can convert documents in markdown, reStructuredText, textile, HTML, DocBook, LaTeX, MediaWiki markup, TWiki markup, OPML, Emacs Org-Mode, Txt2Tags, Microsoft Word docx, LibreOffice ODT, EPUB, or Haddock markup

### plain text
* [ack](https://beyondgrep.com/) Designed for programmers with large heterogeneous trees of source code.
* [sed](skills/sed.md) 
* [perl](skills/perl.md)
* [awk](skills/awk.md)

### json

* [jq](https://stedolan.github.io/jq/)

### plist 

* [defaults](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/defaults.1.html) Defaults allows users to read, write, and delete Mac OS X user defaults from a command-line shell. Mac OS X applications and other programs use the defaults system to record user preferences and other information that must be maintained when the applications aren't running (such as default font for new documents, or the position of an Info panel). Much of this information is accessible through an appli-cation's application's cation's Preferences panel, but some of it isn't, such as the position of the Info panel. You can access this information with defaults

* [plutil](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/plutil.1.html) plutil can be used to check the syntax of property list files, or convert a plist file from one format to another.  Specifying - as an input file reads from stdin.

### xml

* [xmllint](http://xmlsoft.org/xmllint.html) The xmllint program parses one or more XML files, specified on the command line as XML-FILE (or the standard input if the filename provided is - ). It prints various types of output, depending upon the options selected. It is useful for detecting errors both in XML code and in the XML parser itself.

## Network

* [you-get](https://github.com/soimort/you-get) is a tiny command-line utility to download media contents (videos, audios, images) from the Web, in case there is no other handy way to do it.
* [netcat](http://man.openbsd.org/OpenBSD-current/man1/nc.1) The nc (or netcat) utility is used for just about anything under the sun involving TCP, UDP, or UNIX-domain sockets. It can open TCP connections, send UDP packets, listen on arbitrary TCP and UDP ports, do port scanning, and deal with both IPv4 and IPv6. Unlike telnet(1), nc scripts nicely, and separates error messages onto standard error instead of sending them to standard output, as telnet(1) does with some.
* [socat](http://www.dest-unreach.org/socat/) is a relay for bidirectional data transfer between two independent data channels. Each of these data channels may be a file, pipe, device (serial line etc. or a pseudo terminal), a socket (UNIX, IP4, IP6 - raw, UDP, TCP), an SSL socket, proxy CONNECT connection, a file descriptor (stdin etc.), the GNU line editor (readline), a program, or a combination of two of these.  These modes include generation of "listening" sockets, named pipes, and pseudo terminals.
