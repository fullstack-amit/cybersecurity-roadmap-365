# ==========================================
# DAY 20 : NMAP THEORY + CHEAT SHEET
# ==========================================

# OBJECTIVE:
# Nmap commands revise karna


# ------------------------------------------
# WHAT IS NMAP?
# ------------------------------------------

# Nmap = Network Mapper
# used for:
# - finding devices
# - scanning ports
# - detecting services
# - identifying vulnerabilities


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# You = police
# Step 1: check who is in area
# Step 2: check which doors are open
# Step 3: identify people inside


# ------------------------------------------
# HOST DISCOVERY
# ------------------------------------------

nmap -sn 192.168.1.0/24
# find live devices


# ------------------------------------------
# BASIC PORT SCAN
# ------------------------------------------

nmap 192.168.1.5
# scan common ports


# ------------------------------------------
# ALL PORT SCAN
# ------------------------------------------

nmap -p- 192.168.1.5
# scan all ports


# ------------------------------------------
# SPECIFIC PORTS
# ------------------------------------------

nmap -p 22,80,443 192.168.1.5
# scan selected ports


# ------------------------------------------
# SERVICE VERSION
# ------------------------------------------

nmap -sV 192.168.1.5
# detect service + version


# ------------------------------------------
# OS DETECTION
# ------------------------------------------

nmap -O 192.168.1.5
# detect OS


# ------------------------------------------
# AGGRESSIVE SCAN
# ------------------------------------------

nmap -A 192.168.1.5
# full scan (OS + version + scripts)


# ------------------------------------------
# STEALTH SCAN
# ------------------------------------------

nmap -sS 192.168.1.5
# less detectable scan


# ------------------------------------------
# NO PING
# ------------------------------------------

nmap -Pn 192.168.1.5
# skip host discovery


# ------------------------------------------
# TIMING
# ------------------------------------------

nmap -T4 192.168.1.5
# faster scan


# ------------------------------------------
# NSE SCRIPTS
# ------------------------------------------

nmap --script=http-title 192.168.1.5
# get website title

nmap --script=vuln 192.168.1.5
# check vulnerabilities


# ------------------------------------------
# COMBO SCAN
# ------------------------------------------

nmap -sS -Pn -T4 192.168.1.5
# advanced scan


# ------------------------------------------
# HACKER WORKFLOW
# ------------------------------------------

nmap -sn    # find hosts
nmap        # scan ports
nmap -sV    # service version
nmap -A     # deep scan
nmap --script # vulnerability


# ------------------------------------------
# QUICK MEMORY LINE
# ------------------------------------------

# Discover -> Scan -> Detect -> Analyze -> Exploit


# ------------------------------------------
# TODAY GOAL
# ------------------------------------------

# revise theory
# understand commands
# memorize cheat sheet

# ==========================================
# DAY 20 COMPLETE ✅
# ==========================================