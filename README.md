Last Modified 09/07/14 — 11:02:26 AM • Scott Haneda • [@cometbus](https://twitter.com/cometbus)

# WatchInstall

This is going to be quick and dirty, the script works, it is not POSIX compliant, some variables could use quoting or parenthesis.

Basically, the premise is that you `chmod u+x watchinstall` and then run it.  A time stamp will be made.  Then it just sits there and waits and asks if you are done with the installation of your software.

When you are done, switch to your shell, and type "Done".  The script will then scan from / of your computer, and compare the file dates for anything newer than when the script was run.

It outputs the results as full file paths to a file on your Desktop.  You can then track those files down, or do a full uninstall by pre-prending an `rm -rf` in-front of each line.

I will add to this and clean it up, it would be nice if others did as well, as it comes in handy for those erg case softwares you just never know about.