# ==========================================
# DAY 17 : NMAP -O & -A
# ==========================================

# OBJECTIVE:
# OS aur aggressive scan samajhna


# ------------------------------------------
# OS DETECTION (-O)
# ------------------------------------------

nmap -O scanme.nmap.org
# detects operating system of target

# what it does:
# - network responses analyze karta hai
# - OS guess karta hai (Linux, Windows, etc.)
# - TCP/IP fingerprinting use karta hai

# sample output:
# OS details: Linux 5.x
# Network Distance: 2 hops


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# Target = Person
# OS = uska phone type

# nmap -O = check Android ya iPhone


# ------------------------------------------
# AGGRESSIVE SCAN (-A)
# ------------------------------------------

nmap -A scanme.nmap.org
# combines multiple scans


# ------------------------------------------
# WHAT -A INCLUDES
# ------------------------------------------

# - OS Detection (-O)
# - Version Detection (-sV)
# - Script Scanning (-sC)
# - Traceroute


# sample output:
# 22/tcp open ssh OpenSSH 8.x
# OS details: Linux
# Service Info: Host: example


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# -A = full background check
# - kaun hai (service)
# - kaunsa phone (OS)
# - kya version (details)
# - kahan se connected (route)


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# Step 1: discover hosts (-sn)
# Step 2: scan ports
# Step 3: detect services (-sV)
# Step 4: detect OS (-O)
# Step 5: full scan (-A)


# ------------------------------------------
# IMPORTANT WARNING
# ------------------------------------------

# -A is noisy
# target system may log your activity

# use only on:
# - your own lab
# - legal targets (like scanme.nmap.org)


# ------------------------------------------
# SECURITY INSIGHTS
# ------------------------------------------

# hide OS details if possible
# keep system updated
# monitor unusual scans
# use IDS / Firewall


# ------------------------------------------
# PRACTICAL TASK
# ------------------------------------------

nmap -O scanme.nmap.org
nmap -A scanme.nmap.org

# observe:
# - OS detected?
# - services?
# - extra info?


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# -O = OS detection
# -A = full aggressive scan
# use = deep reconnaissance

# ==========================================
# DAY 17 COMPLETE ✅
# ==========================================