<p align="center">
  <img src="logo.png" alt="Teolyth Logo" width="200" style="border-radius: 16px;" />
</p>

<h1 align="center">💠 Teolyth</h1>
<h3 align="center">The First All-in-One Management Panel Focused on Community Growth & Economy (Beta)</h3>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License" /></a>
  <img src="https://img.shields.io/badge/Status-Beta-orange.svg" alt="Beta" />
  <img src="https://img.shields.io/github/languages/top/Teolyth/Teolyth.svg" alt="Languages" />
</p>

---

### 🚀 Overview

**Teolyth** is built to redefine how Discord communities grow and monetize.  
It lets any server owner launch a **premium storefront**, **automate rewards**, and **engage members** through a rich ecosystem of tools inspired by **Shopify**, **Steam**, **Reddit**, and **CS:GO**.

> No technical experience required — build your brand, sell perks, and automate community economies all from one dashboard.

---

### 🌟 Why Teolyth Exists

- 💼 **Founder-first monetisation** – platform owners earn from every connected guild.  
- 💰 **Server-owner revenue** – monetize roles, tiers, channels, and community perks.  
- ⚡ **Automatic delivery** – instant role, coin, or reward assignment.  
- 🧩 **Unified infrastructure** – storefronts, automation, and moderation in one place.  
- 🌍 **Inspired by ecosystems** – merges the best of Discord, Shopify, Reddit, and Steam.

---

## 🧭 Core Feature Matrix

### 🛡️ Moderation & Security
- Warn, list, and clear warnings via `/staffwarn` with auto role removal.
- Timeout, mute, kick, ban, nickname controls.
- Automod filters: links, files, images, invites, ghost pings, spam, mentions, attachments.
- Raid defense, sanction logs, join/leave audits, dashboard monitoring.
- Invite tracking, leaderboards, rewards, and analytics.

### 🧑‍💼 Staff Operations
- Staff analytics: message count, moderation, tickets, voice metrics.
- Role thresholds, weight overrides, and performance charts.
- Staff warning logs (MongoDB-backed) with dashboard badges.
- Quality event logging and dashboard inbox for ticket/tag management.

### 🎟️ Tickets & Support
- Button-based ticket creation with categories and auto transcripts.
- Category-based staff routing and dashboard-integrated controls.

### 💸 Economy, Marketplace & Case Openings
- Coins, XP, leaderboards, auto-roles, streaks.
- Marketplace with dynamic pricing, trading, and storefront editing.
- Case openings with animated sequences and role/item drops.
- Unified logs for marketplace, cases, and currency flow.

### 📨 Messaging & Content Tools
- Visual embed builder with live preview and saved templates.
- News & announcement scheduler with targeted delivery.

### 🖥️ Dashboard & Admin Utilities
- Permission-aware guild selector.
- Activity feeds, audit logs, premium gating, billing, and storefront sync.
- Role/permission matrices, staff application forms, and global branding settings.

### ⚙️ Automations & Data Layers
- Plan & subscription management (Stripe, Revolut).
- Billing, invoices, premium enforcement, and overrides.
- Admin marketplace suite, economy analytics, and trade summaries.
- Guild overview with metrics, quick links, and health indicators.

### 💎 Premium & Monetisation
- Premium plans with per-module gating.
- Super-admin global oversight tools and billing overrides.
- Monetisable modules (marketplace, cases, boosters) per plan.

### 📊 Dashboard Modules
> *Available via the Admin or Super Admin panels.*

`Activity Insights • Admin Plans • Automod • Billing • Cases • Dashboard • Economy • Guilds • Invites • Levels • Messaging • News • Payments • Plans • Profile • Roles • Security • Settings • Staff Apps • Staff Inbox • Staff Activity • Tickets • Storefront • Super Admin • Support Utilities`

---

## ⚠️ Example: Staff Warning Flow

1. Configure a warning role and limit in **Staff Activity → Configuration**.  
2. Issue a warning:
   ```bash
   #staffwarn <staff> reason:"Missed three shifts"

   ```
3. Dashboard logs the event; the Staff Activity table updates with live counts/history.
4. On reaching the limit, the configured staff roles are removed automatically and the warning role is applied.

---

## License

Distributed under the **MIT License**. See [LICENSE](LICENSE) for details.

---

Built with love for Discord communities by the Teolyth team / Azyreh.


