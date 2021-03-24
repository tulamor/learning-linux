
<pre>
  w    # Show who is logged in and what processes are running  
who    # Less information than "w" 

## Processes
top    # Display dynamic real-time information about running processes  
htop   # An enhanced version of top  
ps aux # List all running processes
## Network
netstat -tupln (netstat is a part of net-tools which is DEPRICATED)
apt-get install net-tools 
netstat    = ss
netstat -r = ip route  
netstat -i = ip -s link  
netstat -g = ip maddr  
</pre>