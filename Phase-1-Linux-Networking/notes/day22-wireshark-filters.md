# ==========================================
# DAY 22 : WIRESHARK FILTERS
# ==========================================

# OBJECTIVE:
# Useful packets filter karna


# ------------------------------------------
# WHAT ARE FILTERS?
# ------------------------------------------

# filters = specific traffic dikhana
# without filter = sab packets
# with filter    = useful packets only


# ------------------------------------------
# TCP PORT FILTER
# ------------------------------------------

tcp.port == 80
# port 80 (HTTP) traffic dikhata hai


# ------------------------------------------
# HTTP FILTER
# ------------------------------------------

http
# only HTTP traffic

# note:
# aajkal mostly HTTPS use hota hai
# isliye http filter me kam data milega


# ------------------------------------------
# IP ADDRESS FILTER
# ------------------------------------------

ip.addr == 192.168.1.1
# specific IP ka traffic


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# Network = Road
# Packets = Vehicles
# Filter = police checking
# only selected vehicles allowed


# ------------------------------------------
# PRACTICAL STEPS
# ------------------------------------------

# Step 1:
# Open Wireshark

# Step 2:
# Select interface (eth0)

# Step 3:
# Start capture

# Step 4:
# Open browser (generate traffic)

# Step 5:
# Apply filters:
dns
tcp.port == 80
http
ip.addr == <target_ip>


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# capture all traffic
# apply filters
# extract important data
# focus on target


# ------------------------------------------
# TROUBLESHOOTING
# ------------------------------------------

# http filter empty?
# Possible reasons:
# - HTTPS use ho raha hai
# - No traffic generated
# - Port 80 closed


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# tcp.port == 80 => port filter
# http          => protocol filter
# ip.addr       => device filter
# goal = find useful data

# ==========================================
# DAY 22 COMPLETE ✅
# ==========================================