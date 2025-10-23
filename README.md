<p align="center" style="margin-bottom: 32px;">
  <img src="logo.png" alt="Teolyth Logo" width="220" style="max-width: 65%; border-radius: 28px; box-shadow: 0 24px 68px rgba(13, 23, 71, 0.45);" />
</p>

<h1 align="center">Teolyth Discord Control Panel (Beta)</h1>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License" /></a>
  <img src="https://img.shields.io/badge/status-beta-orange.svg" alt="Beta" />
</p>

<p align="center" style="font-size: 18px; max-width: 860px; margin: 0 auto 48px; color: #1f2937; line-height: 1.6;">
  Teolyth is on track to be one of the boldest projects in the Discord ecosystem — empowering any server owner to launch a
  premium storefront, automate rewards, and keep their community engaged with a constant stream of innovative mechanics.
</p>

<p align="center" style="font-size: 16px; max-width: 760px; margin: 0 auto 52px; color: #4b5563;">
  Without technical experience, a guild can stand up its own brand page, manage subscriptions, drop CS:GO-inspired cases,
  orchestrate Steam-like inventories, and roll out Reddit-style community programmes — all inside a single secure platform.
</p>

---

## Why Teolyth Exists

- **Founder-first monetisation** – premium plans let the platform owner earn a share from every connected guild.
- **Server-owner revenue** – owners monetise their communities with access tiers, custom roles/channels, and in-server economies.
- **Automatic delivery** – coins, roles, channel gates, and rewards are assigned instantly when members subscribe, buy, or trade.
- **Unified infrastructure** – instead of juggling Shopify, Patreon, tip jars, and separate bots, Teolyth centralises storefront, community, and automation under one roof.
- **Built for ecosystems** – combines ideas inspired by Shopify storefronts, Reddit moderation, CS:GO case openings, Discord management, and Steam inventory systems into a cohesive, secure stack.

---

## Core Feature Matrix

### Moderation & Security
- Warn, list, and clear warnings plus the **`/staffwarn`** command with automatic staff-role removal at a configurable limit.
- Timeout, mute/unmute, kick, ban/unban, nickname control, warning cleanup.
- Automod shields: suspicious links, file uploads, images, invites, ghost pings, spam buckets, mass mention caps, line limits, attachment throttling with channel/role whitelists.
- Raid defence hooks, sanction sharing, moderation & security logs, join/leave audit, role-change history, realtime dashboard feed.
- Invite intelligence: inviter tracking, leaderboards, invite rewards, dashboard role rewards.

### Staff Operations
- Staff activity analytics across messages, tickets, moderation, voice, quality feedback.
- Per-role thresholds, weight overrides, primary metric tracking, charts/timeline, aggregated totals.
- Staff warning history stored in MongoDB; dashboard badges with tooltips for latest actions and moderators.
- Quality events logging (positive/negative) with quick-add button in the dashboard.
- Optional staff inbox module for multi-channel support queues, tagging, assignment, export, transcript and plan indicators.

### Tickets & Support
- Button-based ticket creation with categories, category-based staff roles, auto transcript saving.
- Ticket controls embedded in the dashboard, staff analytics integration, transcript viewer/export.

### Economy, Marketplace & Case Openings
- Coins and XP leveling with leaderboards, level-based auto-roles, currency customization, bank settings, streak multipliers.
- Marketplace: buying/selling server perks, dynamic pricing, trading flows, admin storefront controls, live dashboard editor.
- Case openings: configurable drop tables, animated opening sequence, role/item rewards, dashboard case manager.
- Economy logs and sinks aligned with marketplace and case modules.

### Messaging & Content Tools
- Visual embed builder with live preview, saved templates, targeted channel publishing.
- News/announcements publisher, scheduled broadcast hooks, panel-managed pinned messages.

### Dashboard & Admin Utilities
- Guild selector with permission-aware access; module availability adapts automatically to plan/subscription state.
- Activity feed, audit logging, premium gating, plan management helpers, admin billing tools, and premium storefront sync.
- Role & permission matrices, staff application workflow (forms, reviewers, managers, auto-role on accept).
- Global settings: branding, locale, bot toggles, embed defaults, security options.

### Automations & Data Layers
- Plan & subscription management (admin plans, owner subscriptions, billing, premium enforcement, plan cache).
- Stripe/Revolut connectors, invoice generation, checkout, billing portal redirects, admin overrides.
- Marketplace admin suite, drop management, inventory snapshots, trade summaries, economy analytics.
- Guild overview: member counts, boosts, premium state, modules enabled, quick jump links.
- Comprehensive logs: moderation, automod, invites, economy, ticket transcripts, staff warnings, dashboard actions.

### Premium & Monetisation
- Premium plans module with quotas, per-plan module gating, realtime plan state broadcasts.
- Super-admin view for multi-guild oversight, billing overrides, news publishing, global announcements.
- Monetisable modules (marketplace, case openings, economy boosters) ready for per-plan toggles.

### Dashboard Modules Available
- Activity insights
- Admin plans
- Admin subscriptions
- Automod
- Billing
- Case manager
- Dashboard overview
- Economy
- Guilds
- Invites
- Levels
- Messaging
- News
- Payments
- Plans
- Profile
- Roles
- Security
- Settings
- Staff applications
- Staff inbox
- Staff activity
- Tickets
- Storefront
- Super-admin panel
- Support utilities

---

## Staff Warning Flow (Example)

1. Configure warning role and limit inside **Staff Activity -> Configuration**.
2. Issue a warning:
   ```bash
   /staffwarn staff:@Moderator motiv:"Missed three shifts"
   ```
3. Dashboard logs the event; the Staff Activity table updates with live counts/history.
4. On reaching the limit, the configured staff roles are removed automatically and the warning role is applied.

---

## License

Distributed under the **MIT License**. See [LICENSE](LICENSE) for details.

---

Built with love for Discord communities by the Teolyth team.


