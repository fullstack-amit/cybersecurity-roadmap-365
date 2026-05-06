# ==========================================
# DAY 18 : NMAP NSE
# ==========================================

# OBJECTIVE:
# Nmap scripts ka use samajhna


# ------------------------------------------
# WHAT IS NSE?
# ------------------------------------------

# NSE = Nmap Scripting Engine
# scripts during scan run karne deta hai

# used for:
# - information gathering
# - vulnerability detection
# - automation

# think:
# "plugins for Nmap"


# ------------------------------------------
# HTTP TITLE SCRIPT
# ------------------------------------------

nmap --script=http-title scanme.nmap.org

# what it does:
# - website title fetch karta hai
# - HTTP/HTTPS ports pe kaam karta hai

# sample output:
# 80/tcp open http
# | http-title: Go ahead and ScanMe!


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# Website = Shop
# Title = shop ka board
# http-title = board pe kya likha hai


# ------------------------------------------
# VULNERABILITY SCAN SCRIPT
# ------------------------------------------

nmap --script=vuln scanme.nmap.org

# what it does:
# - multiple vulnerability scripts run karta hai
# - known security issues check karta hai
# - possible weaknesses report karta hai

# sample output:
# | vulners:
# | CVE-XXXX-XXXX
# | Possible vulnerability found


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# House check:
# - door weak hai?
# - window broken hai?
# - lock strong hai?

# vuln script = full safety check


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# Step 1: scan ports
# Step 2: detect services
# Step 3: run NSE scripts
# Step 4: find vulnerabilities

# NSE = automation of hacking recon


# ------------------------------------------
# IMPORTANT WARNING
# ------------------------------------------

# vuln scan = noisy
# can trigger alerts

# use only on:
# - your lab
# - legal targets (scanme.nmap.org)


# ------------------------------------------
# SECURITY INSIGHT
# ------------------------------------------

# keep software updated
# patch vulnerabilities
# monitor logs
# disable unnecessary services


# ------------------------------------------
# PRACTICAL TASK
# ------------------------------------------

nmap --script=http-title scanme.nmap.org
nmap --script=vuln scanme.nmap.org

# observe:
# - website title?
# - any vulnerabilities found?


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# NSE = Nmap scripts
# http-title = website info
# vuln = vulnerability scan
# use = automated recon

# ==========================================
# DAY 18 COMPLETE ✅
# ==========================================