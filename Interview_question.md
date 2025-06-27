# Firewall Interview Questions

---

### 1. What is a firewall?
A firewall is a network security device or software that monitors and filters incoming and outgoing network traffic based on predefined rules.

---

### 2. Difference between stateful and stateless firewall?
- **Stateful Firewall**: Tracks the state of active connections and makes decisions based on context.
- **Stateless Firewall**: Evaluates each packet independently without memory of previous packets.

---

### 3. What are inbound and outbound rules?
- **Inbound Rules**: Control traffic coming *into* your system.
- **Outbound Rules**: Control traffic going *out from* your system.

---

### 4. How does UFW simplify firewall management?
UFW (Uncomplicated Firewall) is a simplified interface for managing `iptables` in Linux, allowing users to enable/disable and configure rules with simple commands.

---

### 5. Why block port 23 (Telnet)?
Telnet transmits data, including passwords, in plaintext. Blocking it prevents potential security breaches due to unencrypted communication.

---

### 6. What are common firewall mistakes?
- Allowing insecure services like Telnet
- Leaving unnecessary ports open
- Not enabling the firewall
- Misconfigured rules that block essential services

---

### 7. How does a firewall improve network security?
Firewalls enforce access control by filtering unauthorized traffic, reducing the attack surface and preventing external threats.

---

### 8. What is NAT in firewalls?
Network Address Translation (NAT) is a method used by firewalls to map private IP addresses to public ones, hiding internal networks from external access.

