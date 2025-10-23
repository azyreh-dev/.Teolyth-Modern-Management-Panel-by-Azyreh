# Teolyth Discord Control Panel (Beta)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/status-beta-orange.svg)]()

Teolyth is an **all-in-one management panel for Discord communities** that ships with a companion bot and a feature-rich dashboard. Everything below is built-in and wired together.

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
- Ticket controls embedded in dashboard, staff analytics integration, transcript viewer/export.

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



