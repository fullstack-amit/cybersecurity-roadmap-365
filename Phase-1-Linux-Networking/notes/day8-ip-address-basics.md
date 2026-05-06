# ==========================================
# DAY 8 : IP BASICS
# ==========================================

# OBJECTIVE:
# Private IP, Public IP, aur Localhost samajhna


# ------------------------------------------
# IP address kya hota hai
# ------------------------------------------

# IP address = network me har device ka unique address

# example:
192.168.1.5

# use:
# device ko identify karne ke liye


# ------------------------------------------
# Private IP (Local Network)
# ------------------------------------------

# private IP = same WiFi / same network ke andar use hota hai

# examples:
192.168.1.5
192.168.1.8
192.168.1.10

# check:
ip a

# ranges:
10.x.x.x
172.16.x.x - 172.31.x.x
192.168.x.x


# ------------------------------------------
# Public IP (Internet Address)
# ------------------------------------------

# public IP = internet pe dikhne wala address

# check:
curl ifconfig.me

# example:
49.xxx.xxx.xxx

# samajh:
# Google / YouTube tera public IP dekh sakte hain
# ISP (Airtel, Jio) public IP deta hai


# ------------------------------------------
# Localhost (127.0.0.1)
# ------------------------------------------

# localhost = apna hi system

127.0.0.1

# test:
ping 127.0.0.1

# meaning:
# system khud ko check karta hai


# ------------------------------------------
# DIFFERENCE
# ------------------------------------------

# Private IP:
# - local network me
# - sirf same WiFi me dikhega

# Public IP:
# - internet pe visible
# - duniya dekh sakti hai

# Localhost:
# - sirf apna system
# - external use nahi


# ------------------------------------------
# ANALOGY
# ------------------------------------------

# Private IP = ghar ke room number
# Public IP = ghar ka address
# Localhost = apne aap se baat


# ------------------------------------------
# FULL PRACTICE
# ------------------------------------------

ip a
curl ifconfig.me
ping 127.0.0.1


# ------------------------------------------
# IMPORTANT RULES
# ------------------------------------------

# 192.168.x.x = private IP
# 127.0.0.1 = localhost
# public IP = ISP deta hai
# same WiFi = same private network


# ------------------------------------------
# QUICK REVISION
# ------------------------------------------

# Private IP = local network
# Public IP = internet
# Localhost = self system

# ==========================================
# DAY 8 COMPLETE ✅
# ==========================================