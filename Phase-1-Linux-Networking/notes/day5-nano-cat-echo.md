# ==========================================
# DAY 5 : NANO + CAT + ECHO
# ==========================================

# OBJECTIVE:
# Text files create aur edit karna


# ------------------------------------------
# nano = file open/edit karna
# ------------------------------------------

# example:
nano file.txt


# ------------------------------------------
# Nano Controls
# ------------------------------------------

# Save:
Ctrl + O

# Confirm:
Enter

# Exit:
Ctrl + X


# ------------------------------------------
# cat = file content dekhna
# ------------------------------------------

# example:
cat file.txt


# ------------------------------------------
# cat = input ko output me print karta hai
# ------------------------------------------

# example:
cat

hello

# exit:
Ctrl + D


# ------------------------------------------
# cat > file.txt = overwrite
# ------------------------------------------

# use:
# Purana content delete ho jayega

# example:
cat > file.txt

hello world

# save + exit:
Ctrl + D


# ------------------------------------------
# cat >> file.txt = append
# ------------------------------------------

# use:
# Existing file me new content add karega

# example:
cat >> file.txt

new line

# exit:
Ctrl + D


# ------------------------------------------
# echo = direct text write karna
# ------------------------------------------

# overwrite:
echo "hello" > file.txt


# append:
echo "new line" >> file.txt


# ------------------------------------------
# IMPORTANT CONCEPTS
# ------------------------------------------

# > = overwrite (danger)

# example:
echo "hi" > file.txt


# >> = append (safe)

# example:
echo "hi" >> file.txt


# ------------------------------------------
# COMMON ERROR
# ------------------------------------------

# quote>
# meaning:
# Quote close nahi hua

# fix:
Ctrl + C


# ------------------------------------------
# PRACTICE WORKFLOW
# ------------------------------------------

# example:
touch notes.txt

nano notes.txt

cat notes.txt

echo "hello" >> notes.txt

cat notes.txt


# ==========================================
# DAY 5 COMPLETE ✅
# ==========================================