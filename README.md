# Task 4: Setup and Use Firewall on Ubuntu (UFW)

## Objective
To configure and test basic firewall rules using UFW (Uncomplicated Firewall) on Ubuntu Linux to understand how network traffic filtering works.

---

## Tools Used
- Ubuntu Linux
- UFW (Uncomplicated Firewall)
- Terminal (Command Line)

---

## Steps Performed

### 1. Check Firewall Status
Verified the current status of UFW to ensure the firewall is active.

### 2. View Existing Rules
Displayed current firewall rules to understand default configurations.

### 3. Block Port 23 (Telnet)
Created a firewall rule to block inbound traffic on port 23 (Telnet) to prevent insecure connections.

### 4. Test Firewall Rule
Attempted to connect to port 23 to verify that the rule is working and the connection is blocked.

### 5. Allow SSH (Port 22)
Added a rule to allow SSH traffic on port 22 for secure remote access.

### 6. Remove Test Rule
Deleted the test rule blocking port 23 to restore the system to its original state.

### 7. Final Verification
Checked the firewall status to confirm all rules are correctly applied and system is clean.

---

## Commands Used

```bash
sudo ufw status verbose
sudo ufw status numbered
sudo ufw enable
sudo ufw deny 23
telnet localhost 23
sudo ufw allow 22
sudo ufw delete deny 23
