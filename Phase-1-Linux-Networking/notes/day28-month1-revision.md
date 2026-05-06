# ==========================================
# DAY 28 : MONTH 1 FULL REVISION
# ==========================================

# OBJECTIVE:
# Pure Month 1 ka revision karna
# Important commands revise karna
# Concepts strong karna


# ==========================================
# LINUX BASICS REVISION
# ==========================================

pwd
ls
ls -la
cd ..
clear

mkdir test
touch file.txt
nano file.txt
cat file.txt

cp a.txt b.txt
mv a.txt new.txt
rm file.txt


# ==========================================
# PERMISSIONS REVISION
# ==========================================

ls -l

chmod 777 file.txt
chmod 644 file.txt
chmod 600 file.txt

sudo chown user file.txt


# ==========================================
# NETWORK REVISION
# ==========================================

ping google.com

ip a

ip route

ifconfig

curl ifconfig.me

ping 127.0.0.1

ip neigh


# ==========================================
# MAC SPOOFING REVISION
# ==========================================

sudo ifconfig eth0 down

sudo macchanger -r eth0

sudo ifconfig eth0 up

ip a


# ==========================================
# TCP vs UDP REVISION
# ==========================================

# TCP:
# reliable + slow

# UDP:
# fast + no guarantee


# ==========================================
# NMAP REVISION
# ==========================================

nmap -sn 192.168.1.0/24

nmap -sV scanme.nmap.org

nmap -O scanme.nmap.org

nmap -A scanme.nmap.org

nmap --script=http-title scanme.nmap.org

nmap --script=vuln scanme.nmap.org


# ==========================================
# WIRESHARK REVISION
# ==========================================

wireshark

# filters:
http
dns
tcp
ip.addr == 192.168.1.1


# ==========================================
# CRYPTOGRAPHY REVISION
# ==========================================

# AES:
# same key encryption

# RSA:
# public/private key encryption


# ==========================================
# HASHING REVISION
# ==========================================

md5sum file.txt

sha256sum file.txt


# ==========================================
# HASHCAT + JOHN REVISION
# ==========================================

hashcat -m 0 hash.txt rockyou.txt

john hash.txt --wordlist=rockyou.txt

john --show hash.txt


# ==========================================
# STEGANOGRAPHY REVISION
# ==========================================

steghide embed -cf image.jpg -sf secret.txt

steghide extract -sf image.jpg


# ==========================================
# QUICK MEMORY LINE
# ==========================================

# Linux
# Networking
# Recon
# Nmap
# Wireshark
# Crypto
# Hashing
# Password Cracking
# Steganography


# ==========================================
# DAY 28 COMPLETE ✅
# ==========================================