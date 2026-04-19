# Changelog

All notable changes to Tempo are documented in this file.
Format follows [Keep a Changelog](https://keepachangelog.com/). Versioning follows [Semantic Versioning](https://semver.org/).

## 1.4.1 — 2026-04-19

### Added
- Notes encryption at rest — titles and content encrypted with AES-256-GCM
- **`desktop`** Tray menu redesign — simplified layout with direct access to notes, calendar sync, and settings
- **`desktop`** New menu bar icon
- Window titles update per-route for macOS time tracker support (Timing, Rize, ActivityWatch)
- What's New carousel catches users up on all missed versions, not just the latest

### Fixed
- Project creation from command palette no longer crashes on edge cases
- Notes mutation errors are now surfaced instead of silently swallowed

### Improved
- Team view performance — scoped cache invalidation and memoized components
- Core queries (statuses, labels, teams, projects) persist between sessions
- Async query persister eliminates hydration races on startup
- Notes overlay split into smaller components for better performance and accessibility
- Smooth editor scrolling with safe-band scroll lock in notes and task descriptions
- ARIA attributes and keyboard navigation improvements across notes

## 1.4.0 — 2026-04-11

### Added
- Personal notes — floating overlay with rich text editing and command-palette switcher
- Share tasks publicly with revocable read-only URLs
- Inline `/timeline` Gantt blocks in task descriptions
- In-app bug/suggestion reporter
- Group by status, person, or priority in side panels
- Last active tracking for org members
- Deep linking via `tempo://` protocol
- Local database replica for instant reads in the desktop app
- Virtual scrolling for large task lists
- Configurable global shortcuts (off by default)
- Auto-update banner in sidebar
- Optimistic updates for all task mutations

### Fixed
- Cross-team project visibility when team slugs collide
- Quick-add dismiss, shadow clipping, and spacing issues
- Slash menu positioning in notes modal
- Window toggle reliability across macOS spaces

### Improved
- Electron 41 security hardening
- Query performance with parallel loaders and skeleton UI
- Shared Tiptap editor across all editors
- Code quality cleanup

## 1.3.1 — 2026-03-25

### Added
- Weekly recap popup every Monday
- Searchable popovers for long dropdown lists
- Decimal time estimates (0.5h)

### Fixed
- Direct task links no longer show "page not found"
- Description editor works immediately on new tasks
- Mentions only show active team members

## 1.3.0 — 2026-03-22

### Added
- Google Calendar two-way sync
- Project deletion with task handling options
- Team images across all views
- Human-readable URLs with custom slugs

### Fixed
- Timezone-dependent date shifting
- Empty group task leaking
- Session staleness after login

## 1.2.0 — 2026-03-20

- New faster backend
- Daily reminders for upcoming due dates

## 1.1.0 — 2026-03-19

- Manual task ordering via drag and drop
- Contextual create flows
- Independent view preferences per page

## 1.0.0 — 2026-03-18

Initial release.
