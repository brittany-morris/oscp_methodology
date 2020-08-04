# oscp_methodology
OSCP Methodology


## Blackbox
#### nmap full tcp port scan
* nmap <ip> -sV -sC -O -T4 --traceroute -p - -oA ~/path/filename

#### Ftp
* service -> exploit
* banner
* default creds
* default creds with nsr
* Anonymous login
* nmap info

#### SSH
* service -> exploit
* banner
* default creds
* default creds with nsr
* nmap info

#### Samba
* nmap info:
  * OS samba
  * Computer name/NetBIOS name
  * Domain name

* service (OS samba or nmap service header (139 & 445)) -> exploit
* nmap -sV -sC --open -T4  -p 139,445 --script=vuln --script-args=unsafe=1 <ip>
* enum4linux
* smbclient
 