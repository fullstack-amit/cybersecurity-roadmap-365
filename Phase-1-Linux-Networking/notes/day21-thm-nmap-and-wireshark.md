# ==========================================
# DAY 21 : THM NMAP ROOM + WIRESHARK
# ==========================================

# PART 1 — THM "NMAP" ROOM


# GOAL:
# Nmap room complete karna aur scanning concepts practice karna


# CORE COMMANDS
nmap -sn 10.10.10.0/24   # host discovery
nmap 10.10.10.10        # basic scan
nmap -sV 10.10.10.10    # service + version
nmap -O 10.10.10.10     # OS detection
nmap -A 10.10.10.10     # aggressive scan
nmap -p- 10.10.10.10    # all ports


# NSE SCRIPTS
nmap --script=http-title 10.10.10.10
nmap --script=vuln 10.10.10.10


# HACKER FLOW
# 1. discover hosts (-sn)
# 2. scan ports
# 3. detect services (-sV)
# 4. identify OS (-O)
# 5. deep scan (-A)
# 6. run scripts (NSE)


# PART 2 — WIRESHARK


# WHAT IS WIRESHARK?
# network packet analyzer
# live network traffic capture karta hai
# packets detail me dikhata hai


# INSTALL
sudo apt update
sudo apt install wireshark


# START
wireshark


# INTERFACE SELECT
# eth0  => wired
# wlan0 => wifi
# tun0  => VPN (important for THM)


# START CAPTURE
# select interface
# click Start


# BASIC FILTERS
http                 # HTTP traffic
dns                  # DNS queries
tcp                  # TCP packets
ip.addr==10.10.10.10  # specific IP


# STOP CAPTURE
# click Stop button


# REAL LIFE ANALOGY
# Nmap = knocking doors
# Wireshark = listening conversations
# Nmap finds targets
# Wireshark sees what they are saying


# HACKER USE
# - analyze traffic
# - capture credentials in insecure traffic
# - understand protocols
# - debug network issues


# SECURITY INSIGHT
# - use HTTPS
# - avoid public WiFi sniffing
# - encrypt sensitive data


# PRACTICAL TASK
# Part 1:
# complete THM Nmap room

# Part 2:
# open Wireshark
# select interface
# start capture
# apply filters (http, dns)


# QUICK SUMMARY
# Nmap = scan targets
# Wireshark = analyze traffic
# together = powerful recon tools

# ==========================================
# DAY 21 COMPLETE ✅
# ==========================================