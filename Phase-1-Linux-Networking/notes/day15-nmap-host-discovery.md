# ==========================================
# DAY 15 : NMAP -sn
# ==========================================

# OBJECTIVE:
# Alive hosts dhoondna using Nmap


# ------------------------------------------
# WHAT IS NMAP?
# ------------------------------------------

# Nmap = Network Mapper
# Used to scan networks & discover devices
# Powerful security tool


# ------------------------------------------
# PURPOSE OF -sn
# ------------------------------------------

# -sn = Ping Scan (No port scan)
# Finds which devices are alive
# Does NOT scan ports
# Fast and safe scanning


# ------------------------------------------
# COMMAND
# ------------------------------------------

nmap -sn 192.168.1.0/24
# /24 = scan full local network


# ------------------------------------------
# WHAT IT DOES
# ------------------------------------------

# - sends ping requests
# - detects active hosts
# - lists IP + status


# ------------------------------------------
# SAMPLE OUTPUT
# ------------------------------------------

# Nmap scan report for 192.168.1.1
# Host is up

# Nmap scan report for 192.168.1.5
# Host is up


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# Network = Building
# Devices = Rooms
# nmap -sn = check which rooms have people inside


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# Step 1: scan network (find live hosts)
# Step 2: select target
# Step 3: perform deeper scan


# ------------------------------------------
# DIFFERENCE: netdiscover vs nmap
# ------------------------------------------

# netdiscover:
# - ARP-based scan
# - works only in local network

# nmap -sn:
# - Ping-based scan
# - more flexible & powerful


# ------------------------------------------
# SECURITY INSIGHT
# ------------------------------------------

# If device responds to ping -> visible on network
# Hackers use this to find targets


# ------------------------------------------
# PRACTICAL TASK
# ------------------------------------------

nmap -sn 192.168.1.0/24

# observe:
# - how many devices are alive?
# - their IP addresses


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# Nmap = network scanner
# -sn = host discovery only
# Output = active devices
# Use = first step in hacking

# ==========================================
# DAY 15 COMPLETE ✅
# ==========================================