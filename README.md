||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||                                                 
 ____            _ _             ____      _       _        ||
/ ___| _ __ ___ (_) | ___       / ___|__ _| |_ ___| |__     ||
\___ \| '_ ` _ \| | |/ _ \ __  | |   / _` | __/ __| '_ \    ||
 ___) | | | | | | | |  __/ __  | |__| (_| | || (__| | | |   ||
|____/|_| |_| |_|_|_|\___|      \____\__,_|\__\___|_| |_|   ||
 -DEVELOPED BY / ISMAIL AHAMED                              ||
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++





#So what is the Smile-catch tool ?
Smile-Catch is a tool developed by using python3 programming language to scan the LAN or PAN network . Using IP range scanner to catch any all the users by pinging their devices one by one.



#What is the meaning of the name ? 
Smile-Catch means when you catch someone guilty with his guilt after investigation and he smiles back to you .



#You may ask what is distinguish your tool and other tools ?
My tool is faster to detect the devices around because doesn't use any form of script or any kind of administrator privilegs which make 
it faster to run and covering larg space because of the wifi adapter . 

#Requirements !
1 - any unix system(kali linux,ubunto,redhat ....) .
2 - wifi adapter . 
3 - python3 .
4 - The ip of the ROUTER .



#Installation !
$ apt-get install python3 && apt-get update python3 
$ git clone https://github.com/thearrival/Smile-catch.git
$ cd Smile-Catch
$ python3 Smile-Catch.py --help


#how it's work ?
Smile-Catch work by typing in the terminal :
python3 Smile-Catch.py --help   # to get the guidance for the usage.

$--fron       # The range of ip addresses to start is, default is 1 
$--to         # The range of ip addresses where to end, default is 254
$--ip         # The mask of addresses to scan, for example 192.168.0, default 192.168.1.*
$--delay      # The delay between pings, default is 0 second 
$--load-file  # To scan ip addresses listed in file
$--stdin      # To gran list of ip addresses from stdin 
$--help       # to get this screen 


#Some examples of usage :

Smile-Catch  -f 100 -t 254 -i 192.168.1.* # scan range from 192.168.1.100 to 192.168.1.254
 Smile-Catch .py -l examples/example-ip-list # scan ip adresses from file
 cat examples/example-ip-list | scan-network -s # scan from stdin
 echo "192.168.1.100,192.168.1.101,192.168.1.102,192.168.1.103,192.168.1.104,192.168.1.107,192.168.1.108" | Smile-Catch  -s # scan from stdin

#home/Ismail/project/Smile-Catch# ./Smile-Catch.py --from=100 --to=110 --ip 192.168.1
Adresses to scan: 10
Ping 192.168.1.{100 to 110}
Delay: 1
192.168.1.100 SMILE-CATCH ^_^ IN 0.0013279914856
192.168.1.101 NO Smile back :( , offline
192.168.1.102 SMILE-CATCH ^_^ IN 0.000174999237061
192.168.1.103 NO Smile back :( , offline
192.168.1.104 NO Smile back :( , offline
192.168.1.105 NO Smile back :( , offline
192.168.1.106 NO Smile back :( , offline
192.168.1.107 NO Smile back :( , offline
192.168.1.108 NO Smile back :( , offline
192.168.1.109 NO Smile back :( , offline
192.168.1.110 NO Smile back :( , offline
