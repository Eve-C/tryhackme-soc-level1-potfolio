# A Day in the Life of a Junior Security Analyst – TryHackMe Write-Up

**Date Completed:** 2025-07-01  
**Difficulty:** Introductory  
**Tools Used:** SIEM Dashboard, IP-SCANNER.THM (simulated reputation lookup)

---

## 🧠 Objective

Simulate the core responsibilities of a Junior SOC Analyst by reviewing alerts, identifying suspicious activity, verifying an external IP address using internal tools, escalating appropriately, and blocking the threat.

---

## 🔍 Summary of Investigation

### 🔔 Key Alerts from SIEM:

| Time | Event |
|------|-------|
| 05:25 | ❌ Unauthorized SSH attempt from `221.181.185.159` |
| 05:27 | ✅ Successful SSH login from the same IP |

These events suggest a brute-force attack or credential compromise, as access was eventually gained by the attacker.

---

### 🌐 IP Reputation Check:
Used the provided simulation tool:
- `IP-SCANNER.THM`

Scan Result:
- `221.181.185.159` found in database
- Confidence of being malicious: **100%**
- ISP: China Mobile Communications Corporation  
- Domain: chinamobileltd.thm  
- Location: Zhenjiang, Jiangsu, China

> 🛡️ *Note: IP address and reputation check are part of a TryHackMe simulation. Included for educational purposes only.*

---

## 🚨 Escalation and Remediation

- ✅ Escalated to **Will Griffin – SOC Team Lead**
- ✅ Added the IP to the **Firewall Block List**

---

## 💡 Key Takeaways

- Practiced reviewing and triaging real-time alerts in a SIEM
- Verified malicious activity through simulated intelligence
- Performed escalation and remediation steps accurately
- Reinforced a typical SOC analyst response process:

- 
---

## 🔗 Room Link

[A Day in the Life of a Junior Security Analyst – TryHackMe](https://tryhackme.com/room/jrsecanalystintrouxo)



