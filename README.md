# Efficient linux shell navigation

## Bash shortcuts
<pre>
CTRL + C  # terminate running command  
CTRL + D  # close current shell session  
TAB       # autocompletion
CTRL + L  # clean screen (scrolls down screen)
CTRL + A  # beginning of the line
CTRL + E  # end of the line
ALT  + F  # goes forwards the line one word at once
ALT  + B  # goes backwards the line
CTRL + R  # reverse search of the shell history | CTRL + G let out of search
sudo !!   # rerun previous command as sudo (!! - bang bang)
CTRL + K  # cut to the end of the line (after cursor)
CTRL + U  # cut to the beginning of the line (before cursor)
CTRL + Y  # contains the last thing that you cut
CTRL + W  # kill word backwards (ignore symbols)

tail -f /var/log/syslog  # tailing the log file
less +F /var/log/syslog  # load the entire file into memory buffer (instead of tail)
SHIFT + F                # bring back back to the end of the file

CTRL+ X + E  # continue editing current shell line in a text editor (uses $EDITOR)
ALT + .      # paste last successful command's argument
reset
</pre>
