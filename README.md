# 🛡️ RRHosting: Security Transparency & Abuse Mitigation Report

### ⚠️ Critical Security Disclosure

This repository is an official security initiative by **RRHosting Administration**. It serves as a public archive of Discord Bot Tokens recovered from unauthorized "Sub-Hosting" and "Bot Maker" services operating in violation of our **Terms of Service (ToS)**.

If your token is listed here, your data has been compromised by a third-party reseller. **RRHosting is proactively publishing these tokens to trigger Discord’s automated "Secret Scanning" system, effectively killing the compromised session to protect your account.**

---

## 🔍 The Investigation: "Plain-Text Negligence"

During a routine infrastructure audit, RRHosting identified a surge in high-risk activity originating from specific container environments. Our investigation revealed that several users (primarily within the Arabic-speaking botting community) were abusing our resources to host "Bot Generation" scripts for unsuspecting customers.

### The Technical Failure:

As shown in our findings, these "services" store sensitive authentication credentials in non-encrypted, plain-text formats (e.g., `settings/tokens.json`).

* **Zero Encryption:** Tokens are stored as raw strings.
* **Mass Exposure:** A single vulnerability in their script exposes *every* customer bot simultaneously.
* **Infrastructure Abuse:** These resellers violate RRHosting's "No Sub-Hosting" policy, creating an unstable environment for legitimate users.

> [!CAUTION]
> **RRHosting does not support, condone, or allow the reselling of our containers for insecure third-party bot hosting.**

---

## ⚖️ Our Enforcement Policy

To maintain the integrity of the Discord API and the safety of our hosting ecosystem, RRHosting has implemented the following protocol:

1. **Detection:** Automated scans identify insecure `.json`, `.env`, and `.txt` files containing bot patterns.
2. **Public Disclosure:** Discovered tokens are committed to this repository.
3. **Automated Invalidation:** By making these tokens public, **Discord's Security Team** is notified via their API monitoring. Discord will then automatically:
* Revoke the compromised token.
* Notify the bot owner via System DM or Email.
* Prevent the "sketchy" reseller from further abusing the bot's permissions.


4. **Permanent Suspension:** The hosting accounts responsible for these leaks are terminated without a refund.



## 🛑 How to Recover

If your bot is listed in our logs, follow these steps immediately:

| Step | Action | Description |
| --- | --- | --- |
| **1** | **Rotate Token** | Generate a new token in the [Discord Dev Portal](https://discord.com/developers/applications). |
| **2** | **Audit Permissions** | Check your bot's "Guilds" list for any unauthorized server joins. |
| **3** | **Migrate Hosting** | Stop using "Reseller" scripts and create a own account on RRHosting  |

---

## 📧 Contact & Support

If you are a bot owner and believe your token was caught in this sweep in error, or if you wish to report a reseller abusing RRHosting infrastructure, please contact us:


* **Discord Support:** https://discord.gg/rrhosting-1204026501977214976




**© 2026 RRHosting Security Team. Protecting the developer ecosystem through transparency.**
