# Make WordPress Training – Office Hours

Monthly video meetings for the [Make WordPress Training](https://make.wordpress.org/training/) team: actionable discussion, concrete task assignment, and onboarding new contributors.

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](LICENSE)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## What are the Office Hours?

A monthly 60-minute video meeting where Training team members and contributors can:

- Ask questions and discuss ongoing projects
- Plan concrete next steps and assign tasks
- Onboard new contributors in a welcoming, face-to-face setting

Read the full proposal: [docs/proposal.md](docs/proposal.md)
Published on the Make WordPress Training blog: [Proposal post – February 3, 2026](https://make.wordpress.org/training/2026/02/03/proposal-monthly-office-hour-meeting-for-make-wordpress-training/)

---

## About This Repository

This is a temporary pilot repository. It was created to organize and document the Office Hours format during a three-month trial period running from April to June 2026. Keeping the pilot work in a separate space allows the format to be tested and refined without affecting the official Training Team infrastructure.

If the team decides to continue Office Hours after the pilot evaluation, the plan is to:

1. Propose the process guide (`handbook/Organizing Office Hours Meetings.md`) as a new page in the [Make WordPress Training Handbook](https://make.wordpress.org/training/handbook/).
2. Submit the proposed changes to existing handbook pages for review by Team Reps and Admins.
3. Transfer this repository and its issue history into the official Training Team structures at [github.com/WordPress/Learn](https://github.com/WordPress/Learn).
4. Archive or close this repository once the transfer is complete.

Until then, this repository is the canonical reference for the Office Hours process. The handbook documents in `/handbook/` reflect the process as it stands at the end of the pilot phase.

---

## Repository Structure

```text
wpt-office-hours/
├── README.md                                            ← This file
├── CONTRIBUTING.md                                      ← How to propose topics, get involved
├── LICENSE                                              ← CC BY-SA 4.0
├── docs/
│   └── proposal.md                                      ← Full proposal with community feedback
├── handbook/
│   ├── Organizing Office Hours Meetings.md              ← Process guide (draft handbook page)
│   ├── Proposed Changes to Existing Handbook Pages.md   ← Proposed updates to existing handbook pages
│   └── README.md                                        ← Directory Overview
├── templates/
│   ├── agenda.md                                        ← Reference template for meeting agendas
│   └── meeting-notes.md                                 ← Reference template for meeting notes
└── .github/                                             ← GitHub configuration (workflows, templates, security)
    ├── PULL_REQUEST_TEMPLATE.md                         ← PR Template
    └── ISSUE_TEMPLATE/
        ├── config.yml                                   ← Issue Config
        ├── document-correction.md                       ← Correction Template
        └── topic-proposal.md                            ← Topic Proposal Template
```

---

## Upcoming Meetings

The date of the next Office Hours meeting is listed on the [Make WordPress Training homepage](https://make.wordpress.org/training/) under **Office Hours**.

*Meeting times rotate to cover different time zones. Past meeting notes are published as blog posts on [make.wordpress.org/training](https://make.wordpress.org/training/).*

---

## Topic Ideas & Kanban Board

Have a topic suggestion? [Open a Topic Proposal issue](https://github.com/rfluethi/wpt-office-hours/issues/new?template=topic-proposal.md) – no GitHub experience needed.

All proposed topics are tracked on the [Project Kanban Board](https://github.com/users/rfluethi/projects/10).

---

## How Meeting Notes Work

1. The moderator creates the meeting agenda as a GitHub issue in [WordPress/Learn](https://github.com/WordPress/Learn/issues) at least 48 hours before the meeting
2. After the meeting, the note-taker posts the draft notes as a comment on the agenda issue
3. Participants have ~48 hours to suggest corrections by commenting on the issue
4. Once approved, notes are published as a blog post on [make.wordpress.org/training](https://make.wordpress.org/training/)

---

## Handbook

The `/handbook` directory contains working documents that support the integration of Office Hours into the Make WordPress Training Handbook:

See [handbook/README.md](handbook/README.md) for more details.

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) – no coding skills required. New to GitHub? There's a beginner-friendly section there too.

---

## WordPress Context

These Office Hours complement the work done on [Learn WordPress](https://learn.wordpress.org/) – the platform the Training team builds and maintains. Meeting discussions often feed directly into new learning materials and contributor workflows.

The Office Hours are also a great entry point if you're attending a [WordCamp](https://central.wordcamp.org/) or [Contributor Day](https://make.wordpress.org/training/handbook/getting-started/contributor-day/) and want to get involved with the Training team.

Participation time is tracked via the [Five for the Future](https://make.wordpress.org/five-for-the-future/) program when you use the correct Slack tags at meeting start and end (see [docs/proposal.md](docs/proposal.md#promotion) for details).

---

## Resources

- [Make WordPress Training Handbook](https://make.wordpress.org/training/handbook/)
- [Learn WordPress](https://learn.wordpress.org/)
- [WordPress Community Code of Conduct](https://make.wordpress.org/handbook/community-code-of-conduct/)
- [Five for the Future](https://make.wordpress.org/five-for-the-future/)
- [WordPress Slack](https://make.wordpress.org/chat/) – join `#training`

---

## Code of Conduct

All participation is governed by the [WordPress Community Code of Conduct](https://make.wordpress.org/handbook/community-code-of-conduct/) and the [Mozilla Community Participation Guidelines](https://www.mozilla.org/en-US/about/governance/policies/participation/).

## License

This repository is licensed under [CC BY-SA 4.0](LICENSE), consistent with Make WordPress community content.

## Contact

- Slack: `#training` on [WordPress Slack](https://make.wordpress.org/chat/)
- Organizer: [@rfluethi](https://profiles.wordpress.org/rfluethi/)
