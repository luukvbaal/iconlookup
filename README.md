<center><a><img src="https://i.imgur.com/tlzF4tG.png"></a></center>

Originally written as a companion plugin to the [nnn](https://github.com/jarun/nnn) file browser.

Expects a directory listing and prepends icons based on the file extension. If the input is in `tree -F` or `ls -F` format, directories, sockets, executables and pipes are also distinguished.

Output is colorized using 8-bit [ANSI](https://en.wikipedia.org/wiki/ANSI_escape_code#Colors) escape codes and currently match default `nnn` colors. Escape codes can be adapted to use [24-bit](https://en.wikipedia.org/wiki/ANSI_escape_code#24-bit) colors too.
