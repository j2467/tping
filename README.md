#tping

Simple script to ping a device with a timestamp next to each ping attempt.

If unreachable, the script makes no movement until a ping is successful. 
This is helpful when troubleshooting as you can see the time when the first
ping went through and hopefully the exact time the device came back up.

How to use: 

1. Type `tping` into the bash command line.
2. It will ask for either an IP address or hostname.
3. It will attempt to connect, and only show movement on the screen once a connection is made, with a timestamp next to those successful ping attempts.

Sometimes it is also helpful to write to a file while also displaying output to the screen. 
Here is the command to do that:

bash tping | my_log_$(date +%Y-%m-%d).txt
- will create a file called my_log_2025-08-05.txt

