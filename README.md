# Teolyth Discord Control Panel (Beta)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Node.js](https://img.shields.io/badge/Backend-Node.js-43853d?logo=node.js&logoColor=white)]()
[![MongoDB](https://img.shields.io/badge/Database-MongoDB-4ea94b?logo=mongodb&logoColor=white)]()
[![Status](https://img.shields.io/badge/status-beta-orange.svg)]()

Teolyth is an **all-in-one management panel for Discord communities**.
It ships with the companion Discord bot and provides a modern web dashboard that keeps
moderation, economy, tickets, invites, marketplace, case openings, and staff analytics in sync.

---

## Highlights

- **Unified dashboard** – visually manage all bot modules, permissions, and live data per guild.
- **Staff operations** – staff activity analytics, staff warning escalation, live logs, quality feedback.
- **Economy & marketplace** – layered XP/coin system with shop, case openings, and configurable rewards.
- **Automated security** – automod, invite tracking, moderation logs, and configurable escalation rules.
- **Premium-ready** – modules and limits adapt automatically based on plan configuration.

---

## Architecture Overview

| Layer | Description |
|-------|-------------|
| `src/commands` | Discord slash + prefix commands (moderation, utility, admin, etc.). |
| `src/handlers` | Runtime logic for events (tickets, automod, staff activity). |
| `src/services` | Domain services (economy, staff-activity, staff-warnings, marketplace, plan cache). |
| `dashboard/` | Bootstrap dashboard served by Express. |
| `dashboard/app` | API routes consumed by the front-end plus dashboard sockets. |
| `dashboard/js` | Vanilla ES modules powering interactive sections. |
| `src/database/schemas` | Mongoose models (members, staff warnings, plans, marketplace, etc.). |

The bot and dashboard run in the same Node.js process and share the MongoDB datastore.

---

## Feature Summary (beta)

### Moderation & Security
- Warn, list, and clear warnings plus the **`/staffwarn`** command with automatic staff role removal at warning limit.
- Timeout, mute/unmute, kick, ban/unban, nickname control.
- Auto-escalation when standard members reach configurable warning caps.
- Automod shields for links, attachments, mentions, spam, ghost pings; live dashboard controls.
- Invite tracking with rewards, join/leave logs, role change audit.

### Staff Activity & Warnings
- Voice, ticket, moderation, quality and message tracking per staff member.
- Configurable thresholds/weights per role with dynamic leaderboards and charts.
- Staff warning history persisted in MongoDB; dashboard shows counts, latest action, and tooltips with reasons.
- Staff warning configuration for role assignment and limit enforcement, synced in real time.

### Tickets & Inbox
- Button-based ticket creation with categories, transcript logs, and staff analytics integration.
- Optional staff inbox interface for multi-channel support queues.

### Economy, Marketplace & Case Openings
- Coins plus XP leveling with role rewards.
- Marketplace for buying/selling server perks using coins.
- Case opening mini-game with animated UI and admin-controlled drop tables.

### Embed Builder & Messaging
- Visual builder with live preview, saved templates, and direct channel publishing.

### Dashboard Utilities
- Guild selector with permission-aware access.
- Live activity feed, premium gating, plan management helpers, admin billing tools.
- Extensive configuration modules (security, automod, economy, roles, staff applications, etc.).

---

## Staff Warning Workflow

1. Define warning role and limit inside **Staff Activity ? Configuration**.
2. Use the bot command:
   ```bash
   /staffwarn staff:@Moderator motiv:"Missed three shifts"
   ```
3. Dashboard logs record the action; the Staff Activity table updates with warning counts and history.
4. When the limit is reached, the configured staff roles are removed automatically and the warning role is applied.

---

## Prerequisites

- Node.js 18+
- MongoDB 6+
- Discord application with bot token, intents enabled
- Optional: Redis (if you enable queues/caching), PM2 for production

---

## Getting Started

```bash
# install dependencies
npm install

# copy environment template, then update tokens/URIs
cp .env.example .env

# start the dashboard + bot in development mode
npm run dev
```

Key environment variables:

| Variable | Description |
|----------|-------------|
| `DISCORD_TOKEN` | Bot token |
| `DISCORD_CLIENT_ID` | Client/Application ID |
| `MONGO_URI` | MongoDB connection string |
| `DASHBOARD_URL` | Base URL for the web panel |
| `SESSION_SECRET` | Express session secret |
| `PREMIUM_WEBHOOK_URL` | (Optional) premium automation |

Check `config/` files for additional module defaults (`automod`, `economy`, etc.).

---

## Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start bot and dashboard with nodemon. |
| `npm run lint` | Run ESLint across the repo. |
| `npm run build` | Bundle dashboard assets (if using a bundler). |
| `node scripts/backfill-billing-plans.js` | Example maintenance job. |

---

## Dashboard Modules (Highlights)

- **Automod** – real-time toggles for protections, whitelists, and attachment throttling.
- **Security** – raid defense, sanction shares, advanced logging targets.
- **Economy / Marketplace / Case Manager** – configure coins, shops, drops.
- **Staff Activity** – configure weights, thresholds, warning role and limit, view analytics.
- **Tickets** – categories, automatic transcripts, staff inbox integration.
- **Super-admin** – premium plans, billing management, guild overview.

Each module exposes REST endpoints under `dashboard/app/` and the front-end logic lives in `dashboard/js/`.

---

## Contributing

1. Fork and create a feature branch.
2. Follow existing ESLint/Prettier rules.
3. Add tests or scripts when possible (see `__tests__` and `scripts/`).
4. Submit a PR with a clear summary and testing notes.

Bug reports and feature requests are welcome via Issues or the support Discord (link in the dashboard footer).

---

## Roadmap (short list)

- Advanced economy logs and analytics.
- Seasonal leaderboards with automated reward distribution.
- Expanded security automation (raid scoring, challenge flows).
- Additional premium modules (marketing, scheduling).

Track progress in `docs/` (for example, `staff-activity-metrics.md`, `raid-shield-operations.md`) and the public roadmap once published.

---

## License

Distributed under the **MIT License**. See [LICENSE](LICENSE) for details.

---

Built with love for Discord communities by the Teolyth team.
