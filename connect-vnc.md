# How to Connect to Jetson through VNC.

1. Connect to the Jetson through ssh 
    ssh curc@jetson-t2

2. Verify wifi is enabled for the jetson 
    ping google.com

3. If wifi is enabled, then run ifconfig to get the IP you need to connect through VNC; it will be the address associated with WLAN0:
    ifconfig

4. Then use vnc server ("Screen Sharing" on mac) to connect to that IP address, and provide the password. 