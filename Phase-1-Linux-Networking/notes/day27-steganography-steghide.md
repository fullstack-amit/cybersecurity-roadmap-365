# ==========================================
# DAY 27 : STEGANOGRAPHY
# ==========================================

# OBJECTIVE:
# Data hide aur extract karna


# ------------------------------------------
# WHAT IS STEGANOGRAPHY?
# ------------------------------------------

# steganography = data ko hide karna

# image normal dikhegi
# andar secret data hoga

# difference:
# Encryption      => data lock
# Steganography   => data hide


# ------------------------------------------
# TOOL: STEGHIDE
# ------------------------------------------

# use:
# file ko image ke andar hide karna
# aur baad me extract karna


# ------------------------------------------
# EMBED (HIDE DATA)
# ------------------------------------------

steghide embed -cf image.jpg -sf secret.txt

# -cf = cover file (image)
# -sf = secret file (jo hide karna hai)

# command run karte time password set hota hai


# ------------------------------------------
# EXTRACT (DATA NIKALNA)
# ------------------------------------------

steghide extract -sf image.jpg

# password dalna padega
# sahi password => file extract
# galat password => fail


# ------------------------------------------
# IMPORTANT POINTS
# ------------------------------------------

# image normal dikhegi
# hidden data visible nahi hota

# WhatsApp / social apps:
# image compress karte hain
# hidden data delete ho sakta hai


# ------------------------------------------
# SECURITY NOTE
# ------------------------------------------

# image open karne se virus spread nahi hota (normal case)
# steganography != malware
# sirf data hide hota hai


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# suspicious image => steghide try karo
# hidden data extract karo


# ------------------------------------------
# REAL LIFE EXAMPLE
# ------------------------------------------

# photo ke andar secret message chhupana
# bahar se normal, andar se hidden


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# steganography = data hide
# steghide embed = hide
# steghide extract = reveal
# password = protection

# ==========================================
# DAY 27 COMPLETE ✅
# ==========================================