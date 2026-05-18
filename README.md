# OpenZenith OSINT

Open-source intelligence platform for Discord - one command to uncover everything.

---

## Invite

**Invite Link:** [Click Here to Invite OpenZenith](https://discord.com/oauth2/authorize?client_id=1286454438307037224&permissions=8&scope=bot)

**Application ID:** `1286454438307037224`

**Permissions:** Administrator (Required for full functionality)

---

## About

OpenZenith is a unified OSINT platform that brings powerful intelligence gathering to Discord. One command handles both ID and username resolution, returning comprehensive profile data, history tracking, and cross-source intelligence.

---

## Features

• ID to username resolution (public access)
• Username to ID resolution (access controlled)
• Full Discord profile metadata
• Username change history tracking
• Global name change history tracking
• Mutual servers detection
• Account creation date from snowflake
• Avatar and banner URLs
• Bio / About Me
• GateKeeper integration for threat data
• Multi-source intelligence aggregation
• Pattern matching for similar usernames
• TXT file export for multiple results
• Rate limiting and abuse detection
• RBAC access control system

---

## Access Levels

| Level | Access |
|-------|--------|
| public | ID resolution only |
| low | Basic username search |
| medium | Username to ID resolution |
| high | Full profile metadata |
| critical | Advanced pattern matching |
| owner | Full system control |

---

## Commands

**Public Commands**

`..dc <id>` - Resolve Discord ID to username
`..mylevel` - Check your access level
`..invite` - Get bot invite link
`..help` - Show help menu

**Low Access**

`..dc <username>` - Basic username search (limited results)

**Medium Access**

`..dc <username>` - Full username to ID resolution

**High Access**

`..dc <username>` - Full profile with metadata
`..sync_stats` - View sync statistics

**Critical Access**

`..dc <username>` - Advanced pattern matching
`..sync_now` - Manual sync from GateKeeper

**Owner Only**

`..grant <id> <level>` - Grant OSINT access
`..revoke <id>` - Revoke OSINT access
`..sync_rebuild` - Full database rebuild
`..abuse_logs` - View abuse detection logs

---

## Example Usage

**ID Resolution (Public)**

Input: `..dc <user_id>`

Output includes: User ID, Username, Global Name, Account Creation Date

**Username Resolution (Medium+)**

Input: `..dc <username>`

Output includes: User ID, Username, Global Name, Account Creation Date, Mutual Servers, Avatar URL, Bio, Username History, Global Name History

---

## Data Sources

OpenZenith aggregates intelligence from:

• Discord API (live profile data)
• OpenZenith cache (resolved users)
• GateKeeper database (threat intelligence)
• Pattern matching (leet speak, character variations)
• Mutual guild detection
