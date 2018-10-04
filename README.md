# pingofdeathscriptkiddy
Simple script for PoD

A PoD script can be easily written in any text editor and used on any network capable device. 
The following lines can be written using Notepad and later converted into a batch file by changing the file extension from .txt to .bat. 

$ :loop

$ ping <IP address/domain name> -l 65500 -w 1 -n 1

$ goto :loop

The usual ping command will send 4 packets of 32 bytes to the IP address with a slightly long timeout for each packet. 
Using -l allows us to modify the packet size and using -w we can set the timeout to a minimum of 1 
since we don’t care about the ping requests coming back to us. 
-n allows us to set the number of packets to be sent when the command is run. 
Since the batch file infinitely loops, we can set it to 1.
