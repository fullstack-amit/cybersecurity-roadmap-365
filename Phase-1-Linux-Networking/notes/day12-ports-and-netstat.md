# ==========================================
# DAY 12 : PORTS & NETSTAT
# ==========================================

# OBJECTIVE:
# Ports ko samajhna aur open ports check karna


# ------------------------------------------
# WHAT IS A PORT?
# ------------------------------------------

# Port = virtual door of a system

# each service runs on a specific port

# open port  => service active
# closed port => no access


# ------------------------------------------
# COMMON PORTS
# ------------------------------------------

80    -> HTTP   (insecure web)
443   -> HTTPS  (secure web)
21    -> FTP    (file transfer)
22    -> SSH    (remote login)
3306  -> MySQL  (database)


# ------------------------------------------
# COMMAND: CHECK OPEN PORTS
# ------------------------------------------

netstat -tuln


# ------------------------------------------
# FLAG BREAKDOWN
# ------------------------------------------

-t => TCP
-u => UDP
-l => Listening ports
-n => Numeric output (fast)


# ------------------------------------------
# SAMPLE OUTPUT
# ------------------------------------------

# tcp 0 0 0.0.0.0:22 0.0.0.0:* LISTEN
# tcp 0 0 0.0.0.0:80 0.0.0.0:* LISTEN

# interpretation:
# 22 => SSH running
# 80 => Web server running


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# System = House
# Ports = Doors
# Open door without lock = Risk


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# Step 1: scan ports
# Step 2: find open ports
# Step 3: attack service

# examples:
# 22   => brute force login
# 3306 => database attack


# ------------------------------------------
# SECURITY BEST PRACTICES
# ------------------------------------------

# close unused ports
# strong passwords
# firewall enable
# monitor regularly


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# Ports = Doors
# netstat = Port checker
# Open port = potential risk

# ------------------------------------------
# PRACTICAL TASK
# ------------------------------------------

netstat -tuln

# observe:
# - which ports are open?
# - which services are running?

# ==========================================
# DAY 12 COMPLETE ✅
# ==========================================