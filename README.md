![Project Logo](logo.png)

<h1 align="center">🎶 Discord All-in-One Panel – Beta</h1>
<h3 align="center">The All-in-One Management Panel Focused on Community Growth & Economy</h3>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/version-0.1.0-blue.svg" /></a>
   <img src="https://img.shields.io/badge/License-MIT-green.svg" />
  <img src="https://img.shields.io/badge/status-beta-orange.svg" />
  <img src="https://img.shields.io/badge/Made%20with-Node.js-green?logo=node.js" />
  <img src="https://img.shields.io/badge/Database-MongoDB-brightgreen?logo=mongodb" />
</p>

---

### 🚀 Overview

**Teolyth** is a next-generation platform redefining how Discord communities grow, manage, and monetize.  
It combines **storefronts**, **economy systems**, **moderation tools**, and **automation layers** inside a single, beautiful dashboard.

> Empower your guilds. Build a brand. Automate growth.  
> Inspired by **Shopify**, **Steam**, **Reddit**, and **CS:GO** — reimagined for Discord.

---

### 🌟 Why Teolyth Exists

- 💼 **Founder-first monetisation** – platform owners earn from every connected guild.  
- 💰 **Server-owner revenue** – monetize roles, tiers, and channels via subscriptions & coins.  
- ⚡ **Automatic delivery** – instant fulfillment of roles, coins, and permissions.  
- 🧩 **Unified infrastructure** – storefronts, automations, and moderation all under one roof.  
- 🌍 **Inspired by ecosystems** – built like Shopify, managed like Discord, scaled like Steam.

---

## 🧭 Core Feature Matrix

### 🛡️ Moderation & Security
- Advanced anti-raid & automod shields.
- Filters for links, invites, ghost pings, images, mentions, and spam.
- `staffwarn` command with automatic role removal & history tracking.
- Sanction logs, audit tracking, and dashboard moderation feed.
- Invite tracking, leaderboards, and inviter rewards.

### 🧑‍💼 Staff Operations
- Staff analytics: moderation, tickets, voice activity, and messages.
- Role thresholds, weighted performance scores, and live charts.
- Quality feedback & staff inbox for support tagging and tracking.
- MongoDB-backed warning history with dashboard badges.

### 🎟️ Tickets & Support
- Button-based ticket creation with categories & staff roles.
- Auto transcript saving, dashboard viewing, and export tools.
- Category-based routing with analytics integration.

### 💸 Economy, Marketplace & Case Openings
- Coins, XP leveling, streaks, and auto-roles.
- Marketplace with trading, pricing, and live storefront editing.
- Animated case openings with rarity tables & reward drops.
- Unified economy logs & analytics.

### 📨 Messaging & Content Tools
- Visual embed builder with real-time preview.
- Scheduled announcements, broadcasts, and pin management.

### 🖥️ Dashboard & Admin Utilities
- Guild selector with permission-aware access.
- Activity feeds, audit logs, billing management, and branding.
- Role matrices, staff application system, and premium controls.

### ⚙️ Automations & Data Layers
- Stripe & Revolut integration for plans, billing, and invoices.
- Marketplace admin suite, economy analytics, and trade summaries.
- Real-time plan enforcement and multi-guild overviews.

### 💎 Premium & Monetisation
- Premium plan gating and quota systems.
- Super-admin dashboard for billing overrides and global broadcasts.
- Monetisable modules (Marketplace, Cases, Boosters).

---

## 🎨 Coming Soon

Teolyth continues to expand — here’s what’s next:

| Feature | Description |
|----------|--------------|
| 🧱 **Custom Storefront Templates** | Edit storefront & marketplace themes visually. |
| 🔁 **Member Trading System** | Trade roles/items/coins between members through inventory sync. |
| 🎁 **Giveaway Engine** | Automatic role, coin, or permission rewards for winners. |
| 🧠 **Adaptive Security AI** | Real-time heuristic anti-raid & spam detection. |
| 🏪 **Expanded Role Marketplace** | Sell or trade configurable server roles for coins. |

---

## ⚠️ Example: Staff Warning Flow

1. Configure a warning role & limit in **Staff Activity → Configuration**.  
2. Issue a warning:
   ```bash
   #staffwarn <staff> reason:"Missed three shifts"
