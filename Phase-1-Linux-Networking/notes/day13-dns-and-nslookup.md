# ==========================================
# DAY 13 : DNS & NSLOOKUP
# ==========================================

# OBJECTIVE:
# DNS aur nslookup ka basic use samajhna


# ------------------------------------------
# WHAT IS DNS?
# ------------------------------------------

# DNS = Domain Name System
# Converts domain name -> IP address

# example:
google.com -> 142.250.xxx.xxx

# humans remember names
# computers use IPs


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# DNS = Phone Contact List
# You search: "Amit"
# Phone dials: actual number

# same:
# You type: google.com
# DNS returns: IP address


# ------------------------------------------
# COMMAND: nslookup
# ------------------------------------------

nslookup google.com
# finds IP of domain


# ------------------------------------------
# USING SPECIFIC DNS SERVER
# ------------------------------------------

nslookup facebook.com 8.8.8.8
# 8.8.8.8 = Google DNS server
# query goes to Google instead of default DNS


# ------------------------------------------
# SAMPLE OUTPUT
# ------------------------------------------

# Server: 8.8.8.8
# Address: 8.8.8.8#53
# Name: facebook.com
# Address: 157.240.xxx.xxx

# meaning:
# DNS server responded with IP


# ------------------------------------------
# DNS RECORD TYPES
# ------------------------------------------

A    => Domain -> IPv4 address
MX   => Mail server info
CNAME=> Alias / nickname of domain


# ------------------------------------------
# EXAMPLES
# ------------------------------------------

# A Record
google.com -> 142.250.x.x

# MX Record
gmail.com -> mail servers

# CNAME
www.google.com -> google.com


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# collect target info using DNS
# find:
# - IP address
# - mail servers
# - subdomains

# helps in reconnaissance phase


# ------------------------------------------
# SECURITY RISKS
# ------------------------------------------

# DNS spoofing (fake IP)
# redirect to malicious site
# data interception


# ------------------------------------------
# SECURITY TIPS
# ------------------------------------------

# trusted DNS use karo (8.8.8.8 / 1.1.1.1)
# suspicious links avoid karo
# HTTPS use karo
# DNS security tools enable karo


# ------------------------------------------
# PRACTICAL TASK
# ------------------------------------------

nslookup google.com
nslookup facebook.com 8.8.8.8

# observe:
# - IP address
# - DNS server used


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# DNS = Internet phonebook
# nslookup = DNS query tool
# Records = A, MX, CNAME

# ==========================================
# DAY 13 COMPLETE ✅
# ==========================================