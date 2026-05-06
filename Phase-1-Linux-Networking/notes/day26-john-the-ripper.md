# ==========================================
# DAY 26 : JOHN THE RIPPER
# ==========================================

# OBJECTIVE:
# Another password cracking tool samajhna


# ------------------------------------------
# WHAT IS JOHN THE RIPPER?
# ------------------------------------------

# John The Ripper = password cracking tool
# Hashcat jaisa hi kaam karta hai
# Hash -> password guess -> match


# ------------------------------------------
# BASIC COMMAND
# ------------------------------------------

john hash.txt --wordlist=rockyou.txt

# hash.txt    => file containing hash
# rockyou.txt  => password wordlist


# ------------------------------------------
# HOW IT WORKS
# ------------------------------------------

# 1. wordlist se password leta
# 2. hash banata
# 3. compare karta
# 4. match => password mil gaya


# ------------------------------------------
# ROCKYOU WORDLIST
# ------------------------------------------

# common passwords list
# fast cracking ke liye use hoti hai


# ------------------------------------------
# SHOW CRACKED PASSWORD
# ------------------------------------------

john --show hash.txt
# cracked password display karega


# ------------------------------------------
# DIFFERENCE (Hashcat vs John)
# ------------------------------------------

# Hashcat => fast (GPU)
# John     => easy + beginner friendly
# dono ka kaam same hai


# ------------------------------------------
# IMPORTANT POINT
# ------------------------------------------

# hash type correct hona chahiye
# wordlist strong hona chahiye


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# weak password => quickly crack
# strong password => difficult


# ------------------------------------------
# ETHICAL USE
# ------------------------------------------

# only use in:
# - lab
# - practice
# - TryHackMe

# unauthorized use illegal


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# John = cracking tool
# Wordlist = password list
# match => password mil gaya

# ==========================================
# DAY 26 COMPLETE ✅
# ==========================================