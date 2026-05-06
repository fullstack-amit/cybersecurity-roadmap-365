# ==========================================
# DAY 16 : NMAP -sV
# ==========================================

# OBJECTIVE:
# Service aur version detect karna


# ------------------------------------------
# WHAT IS -sV?
# ------------------------------------------

# -sV = Service Version Detection
# Detects which service is running
# Also shows version of that service


# ------------------------------------------
# COMMAND
# ------------------------------------------

nmap -sV scanme.nmap.org
# scanme.nmap.org = safe test server


# ------------------------------------------
# WHAT IT DOES
# ------------------------------------------

# - scans open ports
# - identifies services
# - detects version


# ------------------------------------------
# SAMPLE OUTPUT
# ------------------------------------------

# PORT STATE SERVICE VERSION
# 22/tcp open ssh  OpenSSH 7.6
# 80/tcp open http Apache 2.4.41


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# Port = Door
# Service = Person inside
# Version = ID card

# nmap -sV = check who is inside + identity


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# Step 1: find open ports
# Step 2: identify service
# Step 3: check version
# Step 4: search vulnerabilities

# Version = key to exploit


# ------------------------------------------
# WHY VERSION IS IMPORTANT
# ------------------------------------------

# old version = vulnerable
# hacker can exploit known bugs

# example:
# Apache 2.2 => vulnerable
# Apache 2.4 => more secure


# ------------------------------------------
# SECURITY INSIGHT
# ------------------------------------------

# always update services
# hide version info if possible
# use firewall


# ------------------------------------------
# PRACTICAL TASK
# ------------------------------------------

nmap -sV scanme.nmap.org

# observe:
# - which ports are open?
# - which services running?
# - which versions?


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# nmap = scanner
# -sV = version detection
# Output = service + version
# Use = find vulnerabilities

# ==========================================
# DAY 16 COMPLETE ✅
# ==========================================