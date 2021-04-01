<center><a><img src="https://i.imgur.com/6AUSXv1.png"></a></center>

Expects a directory listing in stdin and prepends icons based on the file extension. If the input is in `tree -F` or `ls -F` format, directories, sockets, executables and pipes are also distinguished.

Output is colorized using [ANSI](https://en.wikipedia.org/wiki/ANSI_escape_code#Colors) escape codes. Default theme is a random selection of [Nord theme](https://www.nordtheme.com/) colors.
