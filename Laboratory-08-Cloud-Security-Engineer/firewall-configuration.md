# Firewall Configuration

### 1. Allow SSH

sudo ufw allow ssh

This command allows SSH connections so administrators can remotely manage the server.

### 2. Set the Default Deny Policy

sudo ufw default deny incoming

sudo ufw default allow outgoing

These commands block incoming traffic by default and allow outgoing traffic.

### 3. Enable the Firewall

sudo ufw enable

This command activates the UFW firewall.

### 4. Allow Port 8080

sudo ufw allow 8080/tcp

This command allows incoming TCP connections on port 8080 so users can access the web application.

### 5. Verify Firewall Rules

sudo ufw status verbose

sudo ufw status numbered

These commands display the firewall status, default policies, and configured rules.

### 6. Why Must SSH Be Allowed First?

If I enable UFW before allowing SSH, remote SSH connections may be blocked by the firewall, which could prevent administrators from accessing the server remotely.
