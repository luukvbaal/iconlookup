<center><a><img src="https://i.imgur.com/6IqmM6P.png"></a></center>

Expects a directory listing in stdin and prepends icons based on the file extension. If the input is in `tree -F` or `ls -F` format, directories, sockets, executables and pipes are also distinguished.

Use for example `tree -faiF --noreport | iconlookup | fzf | sed 's/.*[[:space:]]//;s/[|=>*]$//'` in your `fzf` command to filter the indicators.

To filter the indicators in your `fzf` preview window add e.g. `--preview="bat -p -f '$(echo {} | sed 's/.*[[:space:]]//;s/[|=>*]$//')' 2>/dev/null"` to your `FZF_DEFAULT_OPTS`

Output is colorized using [ANSI](https://en.wikipedia.org/wiki/ANSI_escape_code#Colors) escape codes. Default theme is a random selection of [Nord theme](https://www.nordtheme.com/) colors.
