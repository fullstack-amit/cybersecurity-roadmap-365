# ==========================================
# DAY 25 : HASHCAT
# ==========================================

# OBJECTIVE:
# Password cracking workflow samajhna


# ------------------------------------------
# WHAT IS HASH CRACKING?
# ------------------------------------------

# hash cracking = original password guess karna
# wordlist se password try + hash compare
# match => password mil gaya


# ------------------------------------------
# HASHCAT TOOL
# ------------------------------------------

# basic command:
hashcat -m <mode> hash.txt /usr/share/wordlists/rockyou.txt


# ------------------------------------------
# ROCKYOU WORDLIST
# ------------------------------------------

gunzip /usr/share/wordlists/rockyou.txt.gz
# common passwords list
# used for cracking


# ------------------------------------------
# HASH TYPES + MODES
# ------------------------------------------

# MD5
hashcat -m 0 hash.txt rockyou.txt

# SHA1
hashcat -m 100 hash.txt rockyou.txt

# SHA256
hashcat -m 1400 hash.txt rockyou.txt

# SHA512
hashcat -m 1700 hash.txt rockyou.txt


# ------------------------------------------
# HASH IDENTIFICATION
# ------------------------------------------

# MD5    => 32 characters
# SHA1   => 40 characters
# SHA256 => 64 characters
# SHA512 => 128 characters

hash-identifier


# ------------------------------------------
# HOW HASHCAT WORKS
# ------------------------------------------

# 1. wordlist se password leta
# 2. hash banata
# 3. compare karta
# 4. match => cracked


# ------------------------------------------
# SPEED
# ------------------------------------------

# CPU => million/sec
# GPU => billion/sec

# output example:
# Speed: 5000 MH/s


# ------------------------------------------
# PASSWORD SPACE
# ------------------------------------------

# formula:
# characters ^ length

# examples:
10^4 = 10,000
36^6 ≈ billions
94^8 ≈ quadrillions


# ------------------------------------------
# PASSWORD STRENGTH
# ------------------------------------------

# weak:
# amit123

# strong:
# T7#kP!9zQ

# best:
# MeraDog@RunsFast7!


# ------------------------------------------
# WHY COMPLEX PASSWORD?
# ------------------------------------------

# capital + number + symbol
# => password space increase
# => cracking difficult


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# weak password => easy crack
# strong password => time lagta

# hacker uses:
# - wordlist
# - patterns
# - brute force


# ------------------------------------------
# IMPORTANT RULE
# ------------------------------------------

# correct hash identify karo
# correct mode use karo
# wrong mode => fail


# ------------------------------------------
# ETHICAL NOTE
# ------------------------------------------

# only use:
# - lab
# - TryHackMe
# - practice

# unauthorized cracking illegal


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# Hashcat = cracking tool
# Mode = hash type
# Wordlist = password list
# strong password = secure
# weak password = cracked

# ==========================================
# DAY 25 COMPLETE ✅
# ==========================================