# ==========================================
# DAY 14 : LINUX FUNDAMENTALS + NETDISCOVER
# ==========================================

# OBJECTIVE:
# Permissions, user types, package management, aur netdiscover


# ------------------------------------------
# FILE PERMISSIONS
# ------------------------------------------

# format:
-rwxr-xr--

# r = read
# w = write
# x = execute

# structure:
# [Owner][Group][Others]

# example:
-rwxr-xr--

# meaning:
# Owner  => read, write, execute
# Group  => read, execute
# Others => read only


# ------------------------------------------
# CHANGE PERMISSIONS
# ------------------------------------------

chmod +x file.sh
# makes file executable


# ------------------------------------------
# USER TYPES
# ------------------------------------------

# Normal User => limited access
# Root User   => full control

whoami
# check current user

sudo su
# switch to root

exit
# root se bahar

Ctrl + D
# alternate exit


# ------------------------------------------
# PROMPT DIFFERENCE
# ------------------------------------------

# => root user
# $  => normal user


# ------------------------------------------
# PACKAGE MANAGEMENT
# ------------------------------------------

sudo apt update
sudo apt install

# example:
sudo apt install netdiscover


# ------------------------------------------
# NETDISCOVER
# ------------------------------------------

# what is netdiscover?
# - tool to find devices in a network
# - shows:
#   IP Address
#   MAC Address
#   Vendor

netdiscover

# scan specific network:
netdiscover -r 192.168.1.0/24
# /24 = full subnet scan


# ------------------------------------------
# SAMPLE OUTPUT
# ------------------------------------------

# IP            MAC Address           Vendor
# 192.168.1.1   xx:xx:xx:xx:xx        Router
# 192.168.1.5   xx:xx:xx:xx:xx        Device


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# Network = Room
# Devices = People
# netdiscover = check who is inside


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# Step 1: scan network
# Step 2: identify targets
# Step 3: attack planning


# ------------------------------------------
# SECURITY INSIGHTS
# ------------------------------------------

# unknown device = risk
# monitor network regularly
# secure WiFi with password


# ------------------------------------------
# PRACTICAL TASK
# ------------------------------------------

whoami
sudo su
exit
netdiscover
netdiscover -r 192.168.1.0/24


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# Linux = system control
# Root = full power
# netdiscover = network scanner
# Recon = first hacking step

# ==========================================
# DAY 14 COMPLETE ✅
# ==========================================