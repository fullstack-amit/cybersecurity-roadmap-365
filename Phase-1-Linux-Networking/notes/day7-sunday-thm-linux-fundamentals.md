# ==========================================
# DAY 7 : NETWORK COMMANDS
# ==========================================

# OBJECTIVE:
# Network dekhna, scan karna, aur basic info samajhna


# ------------------------------------------
# ping = connection test
# ------------------------------------------

ping google.com
# continuous ping
# Ctrl + C to stop

ping -c 4 google.com
# sirf 4 packets

ping 8.8.8.8
# direct IP ping

ping -c 2 8.8.8.8
# limited IP ping


# ------------------------------------------
# ip a = network details
# ------------------------------------------

ip a
# full network info

ip a | grep inet
# sirf IP address lines

ip a | grep eth
# eth interface check

ip a | grep wlan
# WiFi check

ip a | grep lo
# loopback check


# ------------------------------------------
# ip route = active route
# ------------------------------------------

ip route
# full route table

ip route | grep default
# active route only

ip route | grep eth
# eth interface route


# ------------------------------------------
# ifconfig = old command
# ------------------------------------------

ifconfig
# full info

ifconfig | grep inet
# IP only


# ------------------------------------------
# NETWORK SCAN (nmap)
# ------------------------------------------

nmap -sn 192.168.1.0/24
# full network scan

nmap -sn 192.168.1.1-20
# small range scan

nmap -sn 192.168.1.5
# single device

nmap -sn 192.168.0.0/24
# different network example


# ------------------------------------------
# QUICK CHECK FLOW
# ------------------------------------------

ip a
ip route
ping -c 4 google.com
nmap -sn 192.168.1.0/24


# ------------------------------------------
# IMPORTANT UNDERSTANDING
# ------------------------------------------

# IP = ek device
# network = devices ka group

# example:
# 192.168.1.5 -> tera system
# 192.168.1.0/24 -> pura network

# range:
# 192.168.1.1 -> 192.168.1.254

# same WiFi = visible
# different WiFi = invisible

# VirtualBox:
# WiFi -> eth0 dikhega


# ------------------------------------------
# OBSERVE KARNA
# ------------------------------------------

# ping:
# reply aa raha ya nahi

# ip a:
# tera IP kya hai

# ip route:
# dev kya hai

# nmap:
# kitne devices mile


# ------------------------------------------
# EXTRA PRACTICE
# ------------------------------------------

ping -c 2 google.com
ip a | grep inet
ip route | grep default
nmap -sn 192.168.1.1-10

# ==========================================
# DAY 7 COMPLETE ✅
# ==========================================