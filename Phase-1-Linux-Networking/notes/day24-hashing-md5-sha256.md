# ==========================================
# DAY 24 : HASHING
# ==========================================

# OBJECTIVE:
# Hashing aur file verification samajhna


# ------------------------------------------
# WHAT IS HASHING?
# ------------------------------------------

# hashing = data ka fingerprint banana

# example:
# "hello" -> 5d41402abc4b2a76b9719d911017c592

# important:
# same input => same hash
# small change => totally different hash


# ------------------------------------------
# IMPORTANT POINT
# ------------------------------------------

# hash file ko change nahi karta
# hash sirf file ka fingerprint hota hai


# ------------------------------------------
# COMMANDS
# ------------------------------------------

md5sum file.txt
# MD5 hash (fast but weak)

sha256sum file.txt
# SHA256 hash (strong and secure)


# ------------------------------------------
# FILE CHANGE EFFECT
# ------------------------------------------

# Step 1:
echo "hello" > file.txt
md5sum file.txt

# Step 2:
echo "hello world" > file.txt
md5sum file.txt

# result:
# hash completely change ho jayega


# ------------------------------------------
# HASH KA USE
# ------------------------------------------

# 1. File verification
# 2. Password storage
# 3. Data integrity check
# 4. Security systems


# ------------------------------------------
# FILE VERIFY (REAL USE)
# ------------------------------------------

# website deti hai:
# SHA256 = abc123xyz

# tum check karte:
sha256sum kali.iso

# compare:
# same => safe
# different => tampered


# ------------------------------------------
# HASH KAHAN MILTA HAI?
# ------------------------------------------

# official sites (Kali, Ubuntu)
# random download sites pe verify mushkil

# agar hash nahi hai:
# => verify nahi kar sakte
# => risk


# ------------------------------------------
# MD5 vs SHA256
# ------------------------------------------

# MD5 => fast, weak
# SHA256 => strong, secure


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# file change => hash change
# hash verify => tampering detect


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# hash = fingerprint
# file change => hash change
# hash verify => security check
# trusted source => hash available

# ==========================================
# DAY 24 COMPLETE ✅
# ==========================================