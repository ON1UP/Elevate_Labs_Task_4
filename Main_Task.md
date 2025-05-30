# Main Task: Firewall Configuration Summary
## 🔧 System Used
- **Operating System:** Kali Linux
- **Firewall Tool:** UFW (Uncomplicated Firewall)

## 🪜 Steps Followed

### Step 1: Install and Check UFW
```bash
  sudo apt update
  sudo apt install ufw
  sudo ufw enable
```
### Step 2: List current Firewall Rules 
```bash
sudo ufw status numebred
```
### Step 3: Block Telnet (Port 23)
```bash
sudo ufw deny 23
```
### Step 4: Test the rule
```bash
telnet localhost (OR your ip in this case 192.168.1.24 ) 23
```
### Step 3: Allow SSH (Port 22)
```bash
sudo ufw allow 22
```
### Step 4: Remove the test block rule to restore original state.
```bash
sudo ufw status numbered
sudo ufw delete <rule_number>  # replace with actual number for port 23 rule
```
![Task_4](https://github.com/user-attachments/assets/b2b547e4-5c97-4a42-9413-e49670c9e146)

