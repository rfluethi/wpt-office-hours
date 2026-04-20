# Changelog

All notable changes to this project are documented in this file.

Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

---

## [0.2.0-beta] – 2026-04-20

### Added

- **`handbook/` directory** with working documents for integrating Office Hours into the Make WordPress Training Handbook:
  - `handbook/Organizing Office Hours Meetings.md` – complete process guide covering planning, running the meeting, creating GitHub issues for action items, and publishing the recap. Intended as a draft for a new handbook page under [Training Team How-To Guides](https://make.wordpress.org/training/handbook/training-team-how-to-guides/).
  - `handbook/Proposed Changes to Existing Handbook Pages.md` – structured list of proposed additions and edits to nine existing handbook pages, plus a proposal for a new GitHub Labels page and a new GitHub Project board under WordPress/Learn.
  - `handbook/README.md` – directory overview with purpose, scope, and status of each document.

### Changed

**`README.md`**
- Repository structure tree updated: `notes/` removed, `handbook/` and `.github/` added with all contained files.
- *Upcoming Meetings* section: replaced hardcoded meeting date table with a reference to the [Make WordPress Training homepage](https://make.wordpress.org/training/), where the next meeting date is always current.
- *How Meeting Notes Work* section: updated to reflect the new workflow (agenda as GitHub issue in WordPress/Learn, notes as comment on the agenda issue, 48h correction window before blog publication).
- New *Handbook* section added, linking to both handbook documents and `handbook/README.md`.

**`templates/agenda.md`**
- Header updated: replaced filename convention note with instructions for creating the agenda as a GitHub issue in [WordPress/Learn](https://github.com/WordPress/Learn/issues); issue title convention `Office Hours Agenda: [DATE]`; apply the **Office Hours** label.
- Meeting structure revised from 4 blocks to 5 blocks with updated time allocations:

  | Old | New |
  |-----|-----|
  | Welcome & Introductions (00:00–05:00, 5 min) | Welcome & Onboarding (00:00–05:00, 5 min) |
  | Topic Overview (05:00–15:00, 10 min) | Brief Introductions (05:00–15:00, 10 min) |
  | Main Discussion (15:00–45:00, 30 min) | Topic Presentation (15:00–25:00, 10 min) |
  | Next Steps & Action Items (45:00–55:00, 10 min) | Open Discussion (25:00–50:00, 25 min) |
  | Open Q&A & Wrap-Up (55:00–60:00, 5 min) | Review, Next Steps & Wrap-Up (50:00–60:00, 10 min) |

- *Before the Meeting* checklist updated: removed blog announcement post and old notes-file steps; added agenda issue creation in WordPress/Learn, Make WordPress meetings calendar entry, and sharing the agenda issue link in Slack.
- *After the Meeting* checklist updated: note-taker now posts draft notes as a comment on the agenda issue instead of creating a file in `/notes/`.

**`templates/meeting-notes.md`**
- Header updated: replaced filename convention note with a *HOW TO USE THIS TEMPLATE* block explaining that notes are posted as a comment on the agenda issue in WordPress/Learn, not saved as a file in this repository.
- Added *Publish as* field clarifying the comment-based workflow.
- Time fields changed from fixed placeholders to flexible `[START]–[END] UTC`.
- Platform field changed from hardcoded `Zoom` to flexible `[Zoom / Jitsi / etc.]`.
- *Status* block rewritten: correction deadline is now inline in the notes header; correction instructions refer to the agenda issue instead of a file.
- *Related links* section added (agenda issue link, additional context links).
- *Meeting Context* section added: 2–4 sentence narrative introduction explaining the meeting's purpose and fit within the bigger picture.

**`CONTRIBUTING.md`**
- *Review Meeting Notes* section rewritten: the review process now points to the agenda issue in WordPress/Learn instead of files in `/notes/`. Instructions updated for commenting on a GitHub issue rather than inline file comments.
- Labels table updated: removed `timezone-APAC` and `timezone-Americas` labels (no assignment mechanism exists); added `correction` label for document correction issues.

**`.github/ISSUE_TEMPLATE/document-correction.md`**
- Example file path replaced with three realistic examples: agenda issue URL, published blog post URL, and a handbook file path.

**`.github/PULL_REQUEST_TEMPLATE.md`**
- Removed checklist item for meeting notes, agendas, and new documents (no longer stored as files in this repo).
- Added checklist item for handbook draft updates (`/handbook/`).
- Removed filename convention check (linked to the now-deleted `notes/README.md`).
- Added process guide consistency check referencing `handbook/Organizing Office Hours Meetings.md`.

### Removed

- **`notes/` directory** and all contained files:
  - `notes/README.md` – instructions for the old file-based notes workflow.
  - `notes/2026-04-18-agenda.md` – agenda file for Meeting 1 (April 18, 2026); superseded by the GitHub issue [WordPress/Learn#3413](https://github.com/WordPress/Learn/issues/3413).

---

## [0.1.0-beta] – 2026-04-18

Initial beta release. Launched for the first Office Hours meeting on April 18, 2026.

### Added

- `README.md` – project overview, repository structure, upcoming meetings table, how meeting notes work, resources.
- `CONTRIBUTING.md` – contributor guide covering topic proposals, note review, pull requests, issues, and GitHub labels.
- `LICENSE` – CC BY-SA 4.0.
- `docs/proposal.md` – full Office Hours proposal with community feedback, published on the Make WordPress Training blog on February 3, 2026.
- `templates/agenda.md` – reusable agenda template for moderators.
- `templates/meeting-notes.md` – reusable notes template for note-takers.
- `notes/README.md` – instructions for filing and publishing meeting notes.
- `notes/2026-04-18-agenda.md` – agenda for Meeting 1 (April 18, 2026).
- `.github/ISSUE_TEMPLATE/topic-proposal.md` – issue template for topic proposals.
- `.github/ISSUE_TEMPLATE/document-correction.md` – issue template for document corrections.
- `.github/ISSUE_TEMPLATE/config.yml` – issue template configuration.
- `.github/PULL_REQUEST_TEMPLATE.md` – pull request template.

---

*This project follows a rolling versioning scheme during the pilot phase (April–June 2026). Breaking changes will be noted explicitly. Minor corrections and formatting fixes may not be logged individually.*
