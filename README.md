 ____            _ _           ____      _       _     
/ ___| _ __ ___ (_) | ___     / ___|__ _| |_ ___| |__  
\___ \| '_ ` _ \| | |/ _ \   | |   / _` | __/ __| '_ \  
 ___) | | | | | | | |  __/   | |__| (_| | || (__| | | |
|____/|_| |_| |_|_|_|\___|    \____\__,_|\__\___|_| |_|
              -DEVELOPED BY / ISMAIL AHAMED                                        
                                                      
# Smile-Catch


Whats in Smile-Catch ?
is a simple IP range scanner tool developed by using python3 programming language
for modern communication project
by Ismail AHAMED and work for both LAN or PAN Network.
AND there is no required root privigiles in Linux.



esmail19980@gmial.com
$ ./scan-network.py --help
scan-network v.2.1 for GNU/Linux. A simple local network scanner.
Usage: scan-network [long GNU option] [option] from [option] to

 --from (-f) range of ip adresses to start, default is 1
 --to (-t) range of ip adresses where to end, default is 254
 --ip (-i) mask of adresses to scan, for example 192.168.1, default 192.168.1.*
 --delay (-d) delay between pings, default is 0 second
 --load-file (-l) scan ip adresses listed in file
 --stdin (-s) grab list of ip adresses from stdin
 --help this screen

Example of usage:
 scan-network -f 100 -t 254 -i 192.168.1.* # scan range from 192.168.1.100 to 192.168.1.254
 scan-network.py -l examples/example-ip-list # scan ip adresses from file
 cat examples/example-ip-list | scan-network -s # scan from stdin
 echo "192.168.1.100,192.168.1.101,192.168.1.102,192.168.1.103,192.168.1.104,192.168.1.107,192.168.1.108" | scan-network -s # scan from stdin

webnull-gentoo-desktop scan-network # ./scan-network.py --from=100 --to=110 --ip 192.168.1
Adresses to scan: 10
Ping 192.168.1.{100 to 110}
Delay: 1
192.168.1.100 responds in 0.0013279914856
192.168.1.101 not responding, offline
192.168.1.102 responds in 0.000174999237061
192.168.1.103 not responding, offline
192.168.1.104 not responding, offline
192.168.1.105 not responding, offline
192.168.1.106 not responding, offline
192.168.1.107 not responding, offline
192.168.1.108 not responding, offline
192.168.1.109 not responding, offline
192.168.1.110 not responding, offline

Changelog:
14.08.2011 (v.2.3) <webnull.www@gmail.com>:
    * Moved from os.popen4 to subprocess.getoutput
    + Added support for Python 3
    + Handling exceptions from threads to notify user that he have not sufficient permissions

30.07.2011 (v.2.2):
    * Changed Python version from python2.7 to python

29.07.2011 (v.2.1):
    + Added changelog and versioning informations
