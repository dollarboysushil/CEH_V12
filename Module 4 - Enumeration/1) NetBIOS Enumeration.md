

![[img_1.png]]

# NetBIOS Enumeration using Windows CL Utilities

## we are attacking metasploitable 2 vm machine using host machine windows 11

## Attacker : Windows 11   192.168.1.65
## Victim : Metasploitable2   192.168.1.90




![Alt Text](Module%204%20-%20Enumeration/images/image_2.png)

# nbtstat -a 192.168.1.90
-a diaplays all the netbios table of a remote computer





![Alt Text](Module%204%20-%20Enumeration/images/image_3.png)
# nbtstat -c
-c lists contents of the netbios name cache of the remote computer



---
---




# NetBIOS Enumeration using NSE Script


## Attacker : Kali Linux   
## Victim : Metasploitable2   192.168.1.90



![Alt Text](Module%204%20-%20Enumeration/images/image_4.png)

# nmap -sV -v --script nbtstat.nse 192.168.1.90

-sv detects the service version
-v (verbose output) includes all hosta and ports in the output