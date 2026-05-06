# ==========================================
# DAY 10 : MAC SPOOFING
# ==========================================

# OBJECTIVE:
# MAC address change (spoof) karna samajhna


# ------------------------------------------
# WHAT IS MAC SPOOFING?
# ------------------------------------------

# MAC spoofing = apna MAC address temporarily change karna

# use:
# privacy
# testing
# security research


# ------------------------------------------
# MANUAL METHOD
# ------------------------------------------

# Step 1: Interface DOWN
sudo ifconfig eth0 down


# Step 2: MAC Address change (random)
sudo macchanger -r eth0


# Step 3: Interface UP
sudo ifconfig eth0 up


# Step 4: Check MAC
ip a


# ------------------------------------------
# MODERN COMMAND METHOD
# ------------------------------------------

sudo ip link set eth0 down

sudo macchanger -r eth0

sudo ip link set eth0 up

ip a


# ------------------------------------------
# IMPORTANT NOTES
# ------------------------------------------

# macchanger -r
# = random MAC generate karega

# ip a
# = current MAC check karega

# permaddr
# = original MAC

# link/ether
# = changed MAC


# ------------------------------------------
# REBOOT EFFECT
# ------------------------------------------

# reboot ke baad:
# MAC wapas original ho jayega


# ------------------------------------------
# REAL UNDERSTANDING
# ------------------------------------------

# MAC = device identity

# spoofing:
# identity temporarily change karta hai


# ------------------------------------------
# PRACTICE
# ------------------------------------------

ip a

sudo ifconfig eth0 down

sudo macchanger -r eth0

sudo ifconfig eth0 up

ip a


# ------------------------------------------
# QUICK SUMMARY
# ------------------------------------------

# MAC spoofing = MAC change
# macchanger = spoofing tool
# ip a = MAC check
# reboot = original MAC restore


# ==========================================
# DAY 10 COMPLETE ✅
# ==========================================