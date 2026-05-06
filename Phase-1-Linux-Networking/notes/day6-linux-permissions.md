# ==========================================
# DAY 6 : LINUX PERMISSIONS
# ==========================================

# OBJECTIVE:
# File aur folder permissions samajhna aur change karna

# ------------------------------------------
# chmod = permission change karna
# ------------------------------------------

# use:
# Kaun read / write / execute kar sakta hai

# permission types:
r = read      # dekh sakta hai
w = write     # edit kar sakta hai
x = execute   # run kar sakta hai

# structure:
owner | group | others

# permission check:
ls -l

# example output:
# -rw-r--r-- 1 fullstack fullstack file.txt

# number system:
7 = rwx
6 = rw-
5 = r-x
4 = r--
0 = ---


# ------------------------------------------
# chmod examples
# ------------------------------------------

chmod 777 file.txt
# sabko full access

chmod 644 file.txt
# owner = read/write, others = read

chmod 600 file.txt
# sirf owner access


# ------------------------------------------
# chown = owner change karna
# ------------------------------------------

sudo chown amit file.txt
# owner = amit

sudo chown amit:amit file.txt
# owner + group change


# ------------------------------------------
# sudo = admin power
# ------------------------------------------

sudo rm file.txt
# force delete / restricted kaam


# ------------------------------------------
# IMPORTANT
# ------------------------------------------

# chmod = change permission
# chown = change owner
# sudo = admin power

# always check:
ls -l


# ------------------------------------------
# PRACTICE
# ------------------------------------------

mkdir testperm
cd testperm
touch file.txt
ls -l
chmod 777 file.txt
ls -l
chmod 600 file.txt
ls -l

# ==========================================
# DAY 6 COMPLETE ✅
# ==========================================