# ==========================================
# DAY 19 : THM + OPENVPN + PING + NMAP
# ==========================================

# OBJECTIVE:
# TryHackMe connect karna aur first scan karna


# ------------------------------------------
# WHAT IS THM?
# ------------------------------------------

# THM = TryHackMe
# online hacking practice platform
# real vulnerable machines
# safe & legal environment


# ------------------------------------------
# OPENVPN CONNECTION
# ------------------------------------------

sudo openvpn yourfile.ovpn

# success message:
# Initialization Sequence Completed

# meaning:
# VPN connected successfully


# ------------------------------------------
# CHECK VPN INTERFACE
# ------------------------------------------

ip a

# look for:
# tun0

# tun0 present => VPN active


# ------------------------------------------
# TARGET MACHINE
# ------------------------------------------

# THM room provides target IP
# example:
10.10.123.45


# ------------------------------------------
# PING TARGET
# ------------------------------------------

ping 10.10.123.45

# output:
# 64 bytes from 10.10.123.45: icmp_seq=1 ttl=63 time=50ms

# meaning:
# machine alive & reachable

# stop:
# Ctrl + C


# ------------------------------------------
# FIRST NMAP SCAN
# ------------------------------------------

nmap 10.10.123.45

# what it does:
# - scans open ports
# - identifies running services

# sample output:
# 22/tcp open ssh
# 80/tcp open http


# ------------------------------------------
# VERSION DETECTION
# ------------------------------------------

nmap -sV 10.10.123.45
# shows service versions


# ------------------------------------------
# DEEP SCAN (OPTIONAL)
# ------------------------------------------

nmap -A 10.10.123.45
# includes:
# - OS detection
# - version detection
# - scripts
# - traceroute


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# VPN = secret tunnel
# Ping = phone call
# Nmap = door checking


# ------------------------------------------
# HACKER WORKFLOW
# ------------------------------------------

# 1. connect VPN
# 2. get target IP
# 3. ping target
# 4. scan ports
# 5. detect services (-sV)
# 6. deep scan (-A)


# ------------------------------------------
# TROUBLESHOOTING
# ------------------------------------------

# if ping fails:
# - check VPN (tun0)
# - check correct IP
# - ensure machine started on THM


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# THM = hacking practice lab
# VPN = network access
# Ping = check alive
# Nmap = scan target
# goal = start reconnaissance

# ==========================================
# DAY 19 COMPLETE ✅
# ==========================================