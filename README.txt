= flac2mp3

* http://github.com/ymendel/flac2mp3

== DESCRIPTION:

flac2mp3 is a command-line program for converting FLAC files into MP3 files.

== FEATURES/PROBLEMS:

flac2mp3 is meant to, as the name implies, convert FLAC files to MP3 files.

It presently requires the `flac` and `lame` binaries to execute, as those are used for the actual conversion.
It moves tags using the flacinfo-rb and ruby-mp3info gems.

flac2mp3 operates on one file at a time. To convert more, try something like

  for f in *.flac; do flac2mp3 "$f"; done

or

  find . -name '*.flac' -exec flac2mp3 {} \;

== REQUIREMENTS:

* flacinfo gem
* ruby-mp3info gem

== INSTALL:

* rake install_gem

== LICENSE:

Copyright (c) 2007 Yossef Mendelssohn

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

