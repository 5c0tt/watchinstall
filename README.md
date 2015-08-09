08.08.2015 — 07:59:40 PM -0700	
Scott Haneda [@scotthaneda](https://twitter.com/scotthaneda)

# WatchInstall

This is going to be quick and dirty — the script works — it is not POSIX compliant — some variables could use quoting or parenthesis, — though I hope not — be careful.

Basically, the premise is that you `chmod u+x watchinstall` and then run it.  A time stamp file will be made.  Then it just sits there and waits and asks if you if you are done with the installation of your software.

When you are done, switch to your shell, and type "Done" or "D".  The script will then scan from / of your computer, and compare the file dates for anything newer than when the script was run.  You should be able to enter in any path to scan from, though ~ will not work so use full paths.  Someone could send me a patch for that and it would be appreciated.

It outputs the results as full file paths to a file on your Desktop.  You can then track those files down, or do a full uninstall by pre-pending an `rm -rf` in-front of each line.

I will add to this and clean it up, it would be nice if others did as well, as it comes in handy for those edge cases where softwares you just never know about needs to be watched a little closer than usual.