<div align="center">

# ⚔️ 𝗞𝗪𝗜𝗦𝗔𝗧𝗭 — 𝗟𝗲𝗴𝗮𝗹 & 𝗗𝗼𝗰𝘂𝗺𝗲𝗻𝘁𝗮𝘁𝗶𝗼𝗻
### `Minecraft Account, Hypixel & Server Explorer for Discord`

[![Discord Bot](https://img.shields.io/badge/Discord-Verified%20App%20Ready-5865F2?style=for-the-badge&logo=discord&logoColor=white)](#)
[![Minecraft](https://img.shields.io/badge/Minecraft-Java%20%26%20Bedrock-57F287?style=for-the-badge&logo=minecraft&logoColor=black)](#)
[![Effective Date](https://img.shields.io/badge/Effective-November%2026%2C%202026-00B0F4?style=for-the-badge)](#)

<br/>

<kbd><a href="#-overview">📖 Overview</a></kbd> •
<kbd><a href="#-terms-of-service">📜 Terms of Service</a></kbd> •
<kbd><a href="#-privacy-policy">🔒 Privacy Policy</a></kbd> •
<kbd><a href="#-contact--support">💬 Contact & Support</a></kbd>

<br/>

> **Quick Links for Discord Developer Portal Verification:**  
> **Terms of Service URL:** `https://github.com/YOUR_USERNAME/kwisatz-legal#terms-of-service`  
> **Privacy Policy URL:** `https://github.com/YOUR_USERNAME/kwisatz-legal#privacy-policy`

</div>

---

## 📖 Overview

**Kwisatz** is a feature-rich Discord utility bot built for the Minecraft and Hypixel communities. It provides real-time account lookups, 3D skin and cape previews, username history aggregation, UUID conversions, live Java & Bedrock server status checks, and ready-to-paste in-game command generators using Discord **Components V2**.

| Feature | Description |
| :--- | :--- |
| **Account & UUID Explorer** | View Mojang profiles, trimmed/dashed/int-array/offline UUIDs, and account metadata. |
| **Name History & Skins** | Inspect historical usernames, 3D skin/cape renders, and raw texture hashes. |
| **Hypixel Integration** | Check live Hypixel online status, recent games, Bedwars/SkyBlock stats, and Watchdog stats. |
| **Server Pinger** | Query live player counts, MOTDs, versions, and software for Java & Bedrock servers. |
| **Command Generator** | Generate `1.20.5+` component and legacy NBT `/give` head & admin commands. |

---

<a id="terms-of-service"></a>
## 📜 𝗧𝗲𝗿𝗺𝘀 𝗼𝗳 𝗦𝗲𝗿𝘃𝗶𝗰𝗲

<sub>**Last Updated:** November 26, 2026 &nbsp;|&nbsp; **Application:** Kwisatz</sub>

By inviting, accessing, or interacting with **Kwisatz** ("the Bot", "the Service") on Discord, you ("User", "you") agree to be bound by these Terms of Service ("Terms"). If you do not agree to these Terms, please discontinue use of the Bot and remove it from your Discord server.

### 1. Eligibility & Discord Compliance
* You must comply with [Discord's Terms of Service](https://discord.com/terms) and [Discord's Community Guidelines](https://discord.com/guidelines) at all times while using the Bot.
* You must meet the minimum age required to use Discord in your country or jurisdiction.
* Server administrators are responsible for ensuring that members in their servers use the Bot in accordance with these Terms.

### 2. Permitted Use & Restrictions
Kwisatz is provided for informational, community, and entertainment purposes related to Minecraft and Hypixel. You agree **not** to:
1. **Abuse or Overload:** Spam commands, automate requests, or intentionally stress-test the Bot or its upstream APIs.
2. **Harassment & Doxxing:** Use player lookup, status tracking, or name history features to harass, stalk, or target any individual.
3. **Exploitation:** Attempt to reverse-engineer, exploit vulnerabilities, bypass rate limits, or disrupt the Bot's infrastructure.
4. **Misrepresentation:** Claim ownership of the Bot or falsely imply official affiliation with Mojang Studios, Microsoft, Hypixel Inc., or Discord Inc.

### 3. Third-Party Services & Trademarks
* Kwisatz retrieves public game and profile data from third-party APIs including **Mojang API**, **Hypixel Public API**, **MC-Heads**, and public Minecraft server query endpoints.
* **Disclaimer of Affiliation:** Kwisatz is an independent community project and is **not** affiliated with, endorsed by, or associated with Mojang Studios, Microsoft Corporation, Hypixel Inc., or Discord Inc.

### 4. Availability & Modifications
* The Service is provided on an **"AS IS"** and **"AS AVAILABLE"** basis without warranties of any kind, whether express or implied.
* We reserve the right to modify, suspend, rate-limit, or discontinue any command, feature, or access to the Bot at any time without prior notice.

### 5. Limitation of Liability
* To the maximum extent permitted by applicable law, the developer(s) of Kwisatz shall not be liable for any direct, indirect, incidental, or consequential damages resulting from your use of, or inability to use, the Bot, including inaccurate third-party API data or temporary downtime.

### 6. Termination of Access
* We reserve the right to restrict or revoke access to Kwisatz for any user or Discord server that violates these Terms or engages in abusive behavior.

---

<a id="privacy-policy"></a>
## 🔒 𝗣𝗿𝗶𝘃𝗮𝗰𝘆 𝗣𝗼𝗹𝗶𝗰𝘆

<sub>**Last Updated:** November 26, 2026 &nbsp;|&nbsp; **Application:** Kwisatz</sub>

Your privacy matters. This Privacy Policy explains what information **Kwisatz** processes, how it is used, how long it is retained, and how you can request data deletion.

### 1. Information We Collect & Process

Kwisatz adheres to strict **data minimization** and only processes data required to execute slash commands and interactive components:

| Data Category | Examples | Purpose | Storage & Retention |
| :--- | :--- | :--- | :--- |
| **Discord Identifiers** | User ID, Guild (Server) ID, Channel ID | Verify component button/menu ownership (`ownerId`), enforce rate limits, and route replies. | Processed in-memory during active interactions; not sold or shared. |
| **Command Inputs** | Queried Minecraft usernames, UUIDs, server addresses (`host:port`) | Fetch requested profile, skin, Hypixel stats, or server status. | Cached temporarily in-memory (TTL cache) to reduce API load. |
| **Minecraft Account Log** | Public Minecraft UUID, resolved username, `firstSeen` timestamp | Power the Bot's local username history log when external history APIs are unavailable. | Stored locally in the Bot's database until deletion is requested. |
| **Diagnostic Error Logs** | Command name, error stack trace, timestamp | Debug crashes and maintain service stability. | Automatically rotated/purged; contains no message content or DMs. |

> **What We Do NOT Collect:** Kwisatz **never** reads, logs, or stores your Discord direct messages (DMs), general server chat messages, passwords, IP addresses, emails, or payment details.

### 2. How We Use Information
We use processed data strictly to:
* Execute slash commands (`/info`, stats, and server lookups) and render Canvas PNG cards.
* Prevent unauthorized users from hijacking another user's active dropdowns or buttons.
* Cache public API responses temporarily to respect Mojang and Hypixel rate limits.
* Diagnose technical errors and prevent abuse.

### 3. Third-Party Data Sharing
* We **do not sell, rent, or trade** any user data to third parties.
* When you run a lookup command, only the requested **Minecraft username, UUID, or server address** (never your Discord User ID or personal Discord details) is transmitted to upstream public APIs (Mojang, Hypixel, skin renderers, or Minecraft server status APIs) to fulfill your request.

### 4. Data Security & Retention
* Temporary API and image caches expire automatically in memory after a short Time-To-Live (TTL) window (typically 30 seconds to 10 minutes).
* Local username history records contain strictly public Minecraft UUIDs and usernames.
* Reasonable technical safeguards are used to restrict database and host access to authorized bot maintainers only.

### 5. Your Rights & Data Deletion Requests
You have the right to request access to or deletion of any stored data associated with your Discord User ID or Minecraft UUID:
* **Opt-Out:** You may stop using the Bot or remove it from your server at any time.
* **Deletion Request:** Contact the Bot developer via the support channels below with your Discord User ID or Minecraft UUID, and your associated records will be permanently deleted within **7 days**.

### 6. Changes to This Policy
* We may update this Privacy Policy from time to time to reflect new features or Discord requirements. Updates will be posted on this page with a revised **"Last Updated"** date.

---

<a id="contact--support"></a>
## 💬 𝗖𝗼𝗻𝘁𝗮𝗰𝘁 & 𝗦𝘂𝗽𝗽𝗼𝗿𝘁

If you have questions about these Terms, need to report abuse, or wish to request data deletion, please reach out:

* **Bot Developer (Discord):** `@your_discord_username` *(replace with your Discord tag)*
* **Support Server:** `https://discord.gg/your-invite` *(replace with your permanent invite link)*
* **GitHub Issues:** Open an issue in this repository

---

<div align="center">
<sub>Made for the Minecraft & Hypixel Community &nbsp;•&nbsp; Not affiliated with Mojang Studios, Microsoft, or Hypixel Inc.</sub>
</div>
