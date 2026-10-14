# Firewall Configuration

## 1. Allow SSH

```bash
sudo ufw allow ssh
```

This command allows SSH connections through port 22 so administrators can remotely access and manage the server.

## 2. Set the Default Deny Policy

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

These commands block incoming connections by default while allowing outgoing traffic from the server.

## 3. Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

This command allows incoming TCP traffic on port 8080 so users can access the Nginx web application.

## 4. Firewall Security Warning

If `sudo ufw enable` is executed before `sudo ufw allow ssh`, remote SSH access may be blocked, potentially locking administrators out of the server.
