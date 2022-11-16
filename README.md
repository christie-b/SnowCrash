# SnowCrash

This project is an introduction to information security.  
This project is composed of 14 levels, each one contains a vulnerability, which, when exploited, will give you a flag needed to access the next level.  
<br/>

## General instructions
To make this project, you will have to use a VMV(64 bits). Once you have started your machine with the ISO provided with this subject, if your configuration is right, you will get a simple prompt with an IP :  
![alt tag](https://user-images.githubusercontent.com/34480775/100728223-923e5880-33c7-11eb-8188-e360404180bf.JPG)  
Then, you will be able to log-in using the following couple of login:password :  
`level00:level00`  
You really shoud use the SSH connection available on port 4242 :  
`$> ssh level00@[VM_IP] -p 4242`  
Once registered, you’re gonna have to find the password that will log you in with the "flagXX" account (XX = current level number).  
Once logged to the "flagXX" account, launch the "getflag" command.  
It will give you the password to connect to the next level (You may not be able to connect to a "flagXX" account - in this case, you will have to find an alternative method, like a command injection on the program depending on its rights, for instance!).  
• Here is a session example :  
![alt tag](https://user-images.githubusercontent.com/34480775/100729210-c403ef00-33c8-11eb-95d5-ff44954aa1d1.JPG)  
• To help you with some levels, you’re gonna have to use external softwares. You should learn how to use the SCP command.  


## Levels
- **level[00-09] :** This is the mandatory part.  
- **level[10-14] :** This is the bonus part.    

*level00* : Caesar cipher  
*level01* : Crack password in /etc/passwd - John The Ripper  
*level02* : Analyze the TCP stream of a pcap file - Wireshark  
*level03* : Path variable manipulation  
*level04* : Perl script exploit  
*level05* : Exploit a cronjob that executes all the binarys located in a folder  
*level06* : Regex /e modifier exploit  
*level07* : Environment variable command injection  
*level08* : Bypass a file name check with changing the file name, or creating a symbolic link  
*level09* : Reverse a cipher  
*level10* : Race condition between access() and open()  
*level11* : Lua script exploit with nc  
*level12* : Arbitrary code execution on a perl script  
*level13* : Modify a register value in GDB to bypass a comparison  
*level14* : Exploit the getflag command - Remove ptrace protection + Modify a register value in GDB to bypass a comparison  
