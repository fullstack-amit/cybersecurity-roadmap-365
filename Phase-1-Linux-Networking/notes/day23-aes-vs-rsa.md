# ==========================================
# DAY 23 : CRYPTOGRAPHY
# ==========================================

# OBJECTIVE:
# AES aur RSA samajhna


# ------------------------------------------
# WHAT IS CRYPTOGRAPHY?
# ------------------------------------------

# cryptography = data ko secure karna

# plain text -> encrypted text -> decrypted text

# example:
# "hello" -> XyZ#12@ -> "hello"


# ------------------------------------------
# SYMMETRIC ENCRYPTION (AES)
# ------------------------------------------

# same key use hoti hai encrypt + decrypt ke liye
# key = secret password

# flow:
# sender:
# encrypt(data, key)

# receiver:
# decrypt(data, key)

# advantages:
# - fast
# - efficient
# - large data ke liye best

# disadvantage:
# - key share karna risky


# ------------------------------------------
# ASYMMETRIC ENCRYPTION (RSA)
# ------------------------------------------

# do keys use hoti hain:
# public key  = sabko de sakte ho
# private key = secret hoti hai

# flow:
# sender:
# encrypt(data, public key)

# receiver:
# decrypt(data, private key)

# advantages:
# - secure key exchange
# - no need to share secret key

# disadvantage:
# - slow


# ------------------------------------------
# REAL LIFE ANALOGY
# ------------------------------------------

# SYMMETRIC (AES):
# ek locker jiska ek hi key hai

# ASYMMETRIC (RSA):
# ek mailbox
# public key = slot
# private key = owner ka key


# ------------------------------------------
# COMBINATION (REAL WORLD USE)
# ------------------------------------------

# real systems use both:
# 1. RSA -> key exchange
# 2. AES -> actual data encryption

# example:
# HTTPS


# ------------------------------------------
# HACKER THINKING
# ------------------------------------------

# weak encryption = attack possible
# strong encryption = secure system

# focus:
# - key strength
# - algorithm type


# ------------------------------------------
# QUICK DIFFERENCE
# ------------------------------------------

# AES => same key, fast
# RSA => two keys, secure but slow


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# cryptography = data protection
# AES = speed
# RSA = security
# together = strong system

# ==========================================
# DAY 23 COMPLETE ✅
# ==========================================