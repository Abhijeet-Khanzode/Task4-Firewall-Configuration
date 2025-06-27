# Windows Firewall - GUI Steps

## Step 1: Open Windows Defender Firewall
- Go to `Control Panel → System and Security → Windows Defender Firewall`
- Click on `Advanced Settings` on the left pane

## Step 2: View Existing Rules
- Inbound and outbound rules are listed in the left-hand side panel.

## Step 3: Create a New Inbound Rule to Block Port 23
- Click `Inbound Rules → New Rule`
- Choose `Port` → Select `TCP` → Enter `23`
- Select `Block the connection`
- Apply to `Domain`, `Private`, and `Public`
- Name it: `Block Telnet Port 23`

## Step 4: Test the Rule
- Open Command Prompt and run:
  ```cmd
  telnet localhost 23
Step 5: Remove the Rule
Go back to Inbound Rules

Find your Block Telnet Port 23 rule

Right-click → Delete

yaml
Copy code

---

### 📄 `linux_ufw_commands.txt`

```bash
# Linux UFW Firewall Configuration (For Reference)

# Enable UFW
sudo ufw enable

# List current rules
sudo ufw status verbose

# Block port 23 (Telnet)
sudo ufw deny 23/tcp

# Test with Telnet
telnet localhost 23

# Allow SSH (Port 22)
sudo ufw allow 22/tcp

# Delete the deny rule
sudo ufw delete deny 23/tcp
