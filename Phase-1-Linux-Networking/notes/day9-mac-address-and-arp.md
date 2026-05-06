# ==========================================
# DAY 9 : MAC ADDRESS + ARP
# ==========================================

# OBJECTIVE:
# MAC address aur ARP ka concept samajhna


# ------------------------------------------
# MAC address kya hota hai
# ------------------------------------------

# MAC = device ka permanent hardware address

# example:
00:1A:2B:3C:4D:5E

# check:
ip a

# important line:
# link/ether xx:xx:xx:xx:xx:xx

# note:
# har device ka MAC alag hota hai


# ------------------------------------------
# IP vs MAC
# ------------------------------------------

# IP = network address (change ho sakta hai)
# MAC = permanent identity (fix hota hai)

# example:
# IP  -> 192.168.1.5
# MAC -> aa:bb:cc:dd:ee:ff


# ------------------------------------------
# ARP kya hota hai
# ------------------------------------------

# ARP = Address Resolution Protocol

# kaam:
# IP se MAC address dhoondna

# note:
# ARP background me chalta hai


# ------------------------------------------
# ARP ka process
# ------------------------------------------

# Step 1:
ping 10.0.2.2

# Step 2:
# system poochta -> iska MAC kya hai?

# Step 3:
# ARP request send hoti hai

# Step 4:
# device reply karta hai

# Step 5:
# MAC mil jata hai


# ------------------------------------------
# MAC kaha dikhega
# ------------------------------------------

ip neigh

# output example:
# 10.0.2.2 dev eth0 lladdr 52:55:0a:00:02:02 REACHABLE

# samajh:
# 10.0.2.2 -> IP
# 52:55:0a:00:02:02 -> MAC


# ------------------------------------------
# IMPORTANT RULES
# ------------------------------------------

# ip a -> apna MAC
# ip neigh -> dusre devices ke MAC

# bina ping:
# MAC nahi milega

# ping:
# ARP ko trigger karta hai

# ARP:
# IP -> MAC convert karta hai


# ------------------------------------------
# STATES
# ------------------------------------------

# REACHABLE = fresh / active
# STALE = old / confirm nahi

# change:
# ping karo -> STALE -> REACHABLE


# ------------------------------------------
# REAL USE
# ------------------------------------------

# kaun network me hai
# device identify
# security check
# troubleshooting


# ------------------------------------------
# PRACTICE COMMANDS
# ------------------------------------------

ip a
ping -c 1 10.0.2.2
ip neigh
ip neigh | grep 10.


# ------------------------------------------
# FINAL UNDERSTANDING
# ------------------------------------------

# IP = naam
# MAC = asli identity
# ARP = naam se aadmi dhoondna
# ping -> ARP ko start karta hai

# ==========================================
# DAY 9 COMPLETE ✅
# ==========================================