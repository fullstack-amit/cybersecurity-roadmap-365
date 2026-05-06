# Linux & Networking Commands Cheatsheet

## 📁 File & Directory
| Command | Kya karta hai |
|---------|--------------|
| pwd | Current location dikhata hai |
| ls -la | Sab files (hidden bhi) dikhata hai |
| mkdir folder | Folder banata hai |
| rm file.txt | File delete karta hai |
| cp file dest | Copy karta hai |
| mv file dest | Move/rename karta hai |
| chmod 755 file | Permission set karta hai |
| chown user file | Owner change karta hai |

## 🌐 Network
| Command | Kya karta hai |
|---------|--------------|
| ifconfig | Network interfaces dikhata hai |
| ip a | IP address dikhata hai |
| ping google.com | Connection test karta hai |
| curl ifconfig.me | Public IP dikhata hai |
| arp -a | ARP table dikhata hai |
| netstat -tuln | Open ports dikhata hai |
| nslookup google.com | DNS lookup karta hai |

## 🔍 Nmap
| Command | Kya karta hai |
|---------|--------------|
| nmap -sn 192.168.1.0/24 | Host discovery |
| nmap -sV target | Service version detect |
| nmap -O target | OS detect |
| nmap -A target | Aggressive scan |
| nmap --script=vuln target | Vulnerability scan |

## 🔐 Hashing & Crypto
| Command | Kya karta hai |
|---------|--------------|
| md5sum file.txt | MD5 hash nikalta hai |
| sha256sum file.txt | SHA256 hash nikalta hai |
| hashcat -m 0 hash.txt rockyou.txt | Hash crack karta hai |
| john hash.txt --wordlist=rockyou.txt | Hash crack karta hai |
| steghide embed -cf img.jpg -sf secret.txt | Data hide karta hai |
| steghide extract -sf img.jpg | Data extract karta hai |