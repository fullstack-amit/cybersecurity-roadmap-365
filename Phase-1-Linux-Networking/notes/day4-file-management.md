# ==========================================
# DAY 4 : FILE MANIPULATION
# ==========================================

# OBJECTIVE:
# Files aur folders create, copy, move, delete karna


# ------------------------------------------
# mkdir = naya folder banana
# ------------------------------------------

# example:
mkdir myfolder


# ------------------------------------------
# Multiple folders banana
# ------------------------------------------

# example:
mkdir test1 test2 test3


# ------------------------------------------
# touch = empty file banana
# ------------------------------------------

# example:
touch file.txt


# ------------------------------------------
# Multiple files banana
# ------------------------------------------

# example:
touch a.txt b.txt


# ------------------------------------------
# rm = file delete karna
# ------------------------------------------

# example:
rm file.txt


# ------------------------------------------
# rm -r = folder delete karna
# ------------------------------------------

# example:
rm -r myfolder


# ------------------------------------------
# rm -rf = force delete (danger)
# ------------------------------------------

# example:
rm -rf test


# ------------------------------------------
# cp = file copy karna
# ------------------------------------------

# syntax:
cp oldfile newfile

# example:
cp a.txt b.txt


# ------------------------------------------
# cp -r = folder copy karna
# ------------------------------------------

# example:
cp -r folder1 folder2


# ------------------------------------------
# mv = rename ya move karna
# ------------------------------------------

# rename example:
mv a.txt new.txt


# move example:
mv new.txt Desktop/


# move to parent folder example:
mv a.txt ../backup/


# ------------------------------------------
# Folder Structure Banana
# ------------------------------------------

# objective:
# /projects/hacking/tools/

# commands:
mkdir projects
cd projects

mkdir hacking
cd hacking

mkdir tools


# ------------------------------------------
# VERIFY STRUCTURE
# ------------------------------------------

# command:
pwd
ls


# ------------------------------------------
# COMMON ERRORS
# ------------------------------------------

# No such file or directory
# meaning:
# File exist nahi karti

# fix:
ls


# Permission denied
# meaning:
# Access nahi hai

# fix:
sudo command


# command not found
# meaning:
# Spelling mistake

# fix:
Correct command name


# ==========================================
# DAY 4 COMPLETE ✅
# ==========================================