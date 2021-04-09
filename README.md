<center><a><img src="https://i.imgur.com/L1WtKjy.png"></a></center>

Expects a directory listing in stdin and prepends icons based on the file extension. If the input is in `tree -F` or `ls -F` format, directories, sockets, executables and pipes are also distinguished.

Use for example `tree -faiF --noreport | iconlookup | fzf | awk '{print /.*[>*|=]$/ ? substr($2, 1, length($2) - 1) : $2}'` in your `fzf` command to filter the indicators.

Output is colorized using [ANSI](https://en.wikipedia.org/wiki/ANSI_escape_code#Colors) escape codes. Default theme is a random selection of [Nord theme](https://www.nordtheme.com/) colors.
