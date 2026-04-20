# Proposed Changes to Existing Handbook Pages

> **Purpose of this document**
> Based on the new process guide [Organizing Office Hours Meetings](Organizing%20Office%20Hours%20Meetings.md), this document lists concrete proposed changes and additions for each existing handbook page. The goal is to ensure the Office Hours format is properly anchored in the existing handbook and that no contradictions or gaps remain.
>
> **Research note:** The sub-pages of *How We Use GitHub* could not be fetched directly via WebFetch. Recommendations for those pages are based on search results, the main page content, and GitHub repository structures. Two additional relevant pages were identified during research: **GitHub Labels** and **Automated Workflows**.

---

## In this document

- [1. Hosting Training Team Meetings](#1-hosting-training-team-meetings)
- [2. How to Write Meeting Agendas and Recap Posts](#2-how-to-write-meeting-agendas-and-recap-posts)
- [3. How We Use GitHub (main page)](#3-how-we-use-github-main-page)
- [4. GitHub Labels *(newly identified)*](#4-github-labels-newly-identified)
- [5. Automated Workflows *(newly identified)*](#5-automated-workflows-newly-identified)
- [6. Triaging Content Development Issues](#6-triaging-content-development-issues)
- [7. Validating and Applying Content Feedback](#7-validating-and-applying-content-feedback)
- [8. Triaging Content Localization Issues](#8-triaging-content-localization-issues)
- [9. Guidelines for Reviewing Content](#9-guidelines-for-reviewing-content)
- [10. New GitHub Project Board *(new infrastructure)*](#10-new-github-project-board-new-infrastructure)
- [Summary: Priority of changes](#summary-priority-of-changes)

---

## 1. Hosting Training Team Meetings

**URL:** https://make.wordpress.org/training/handbook/training-team-how-to-guides/hosting-training-team-meetings/

### What the page currently covers

The page describes two meeting formats: the weekly Slack-based Team Meetings and the Coffee Hours (informal video calls with no agenda).

### Problem

Office Hours exist as a third, distinct meeting format that is not mentioned anywhere on this page. Office Hours have replaced Coffee Hours as the team's primary video format. Someone reading this page has no way of knowing that Office Hours exist or how they differ from Coffee Hours.

### Proposed changes

**A. Update the page introduction**

Expand the opening sentence to include Office Hours:

> **Current:** *"The Training Team alternates between official Team Meetings and casual Coffee Hours each week in the #training Slack channel."*
>
> **Proposed:** *"The Training Team holds weekly Slack-based Team Meetings, occasional informal Coffee Hours, and a monthly Office Hours video meeting. You can see the current meeting times in the welcome box on Make.WordPress.org/Training."*

**B. Add a transition note to the Coffee Hours section**

At the start of the *Hosting Coffee Hours* section:

> **Note:** As of April 2026, the Training Team introduced Office Hours as the team's primary structured monthly video meeting. Coffee Hours may still be held as informal, social sessions, but are no longer the main video format. See [Hosting Office Hours](#hosting-office-hours) below.

**C. Add a new "Hosting Office Hours" section**

Insert after the Coffee Hours section:

---

**Hosting Office Hours**

Office Hours are the Training Team's monthly 60-minute structured video meetings on Zoom. Unlike Coffee Hours, they follow a fixed agenda and every session produces concrete action items tracked as GitHub issues. Moderation and note-taking rotate among team members.

For the complete process (including how to prepare the agenda, run the meeting, create GitHub issues, and publish the recap), see: [Organizing Office Hours Meetings](https://make.wordpress.org/training/handbook/training-team-how-to-guides/organizing-office-hours-meetings/)

**Quick reference for moderators:**
- Post `<office hour meeting>` in `#training` with the Zoom link when the meeting starts (logs time for [Five for the Future](https://make.wordpress.org/five-for-the-future/)).
- Post `</office hour meeting>` in `#training` when the meeting ends.
- Announce the meeting in `#training` at least one week and again 24 hours before.
- At least one Team Representative should be present at each session.

---

---

## 2. How to Write Meeting Agendas and Recap Posts

**URL:** https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-to-write-a-meeting-agenda-or-recap/

### What the page currently covers

The page describes the agenda and recap process for weekly Slack-based Team Meetings: agenda as a GitHub issue, recap post on the Training Team blog.

### Problem

The Office Hours process differs from the described standard process in several important ways:

| Point | Standard meeting (Slack) | Office Hours |
|-------|--------------------------|--------------|
| Agenda | GitHub issue, Meeting Agenda template | GitHub issue, Meeting Agenda template + **Office Hours label** |
| Recap draft | Directly as a blog post draft | First as a **comment on the agenda issue**, 48h correction window |
| Recap scope | Short summary of Slack discussion | Detailed document with narrative discussion summary, decisions table, full action items table |
| Announcement | Make Training blog + Slack | **Slack only** |

Someone following the current guide for an Office Hours recap would skip the 48h draft step and publish directly to the blog, which is incorrect.

### Proposed changes

**A. Expand the introduction**

In the *Volunteering to create a meeting agenda or recap notes* section, add:

> **Note:** This page covers the process for weekly Slack team meetings. For the monthly Office Hours video meetings, the agenda and recap process differs in several ways. See [Publishing Office Hours Agendas and Recaps](#publishing-office-hours-agendas-and-recaps) below, or the full guide: [Organizing Office Hours Meetings](https://make.wordpress.org/training/handbook/training-team-how-to-guides/organizing-office-hours-meetings/).

**B. Add a new section "Publishing Office Hours Agendas and Recaps"**

Recommended location: after the *Publishing Training Team Meeting Agendas* section.

---

**Publishing Office Hours Agendas and Recaps**

**Agenda**

Office Hours agendas are published as GitHub issues in `WordPress/Learn`, using the same **Meeting Agenda** template as regular meetings. Two differences apply:

1. Apply the **Office Hours** label to the issue.
2. Publish the agenda **at least 48 hours before the meeting**, not just a few days before, to give non-native English speakers time to prepare.

Do not publish a separate announcement post on the Make Training blog. Instead, share the agenda issue link in the `#training` Slack channel one week before and again 24 hours before the meeting.

**Recap**

Office Hours recaps are published on make.wordpress.org/training, but include an additional draft step before the blog post is created:

1. **Write the draft as a comment on the agenda issue.** Use the [meeting notes template](https://github.com/rfluethi/wpt-office-hours/blob/main/templates/meeting-notes.md) as your structural guide.
2. **Share the issue link in `#training`** so participants can suggest corrections.
3. **Allow approximately 48 hours** for corrections before publishing to the blog.
4. Then follow the standard blog post publication process described above.

Office Hours recaps are more detailed than standard meeting recaps. They include:
- A narrative discussion summary for each topic (not just bullet points)
- A formal decisions table
- A full action items table with links to GitHub issues
- A follow-up section reviewing open items from the previous meeting

---

**C. Expand the "Points to Remember" section**

Add the following bullet point:

> - For **Office Hours** recaps: always write the draft as a comment on the agenda issue first, allow 48 hours for corrections, and only then create the blog post draft.

---

## 3. How We Use GitHub (main page)

**URL:** https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/

### What the page currently covers

Overview of the `WordPress/Learn` repository: project boards, issue templates, triage processes. The main page lists six use cases for the repository.

### Problem

The Office Hours format generates two new issue types in the same repository that are not described in any of the existing categories. Without documentation, triage members risk incorrectly assigning these issues.

### Proposed changes

**A. Expand the repository use case list in the intro**

Add one new item to the existing list:

> - Issues tracking content development for Learn WordPress
> - Issues tracking content translation for Learn WordPress
> - Issues tracking content topic ideas for Learn WordPress
> - Issues tracking admin tasks of the Training Team
> - Learn WordPress site bugs, content feedback, and other communication from learners
> - **Issues tracking Office Hours meeting agendas and action items** *(new)*

**B. Add a new "Office Hours Issues" section**

Recommended location: after *Use sub-issues*, before *Triaging project boards*.

---

**Office Hours Issues**

The monthly Office Hours video meeting generates two types of issues in `WordPress/Learn`, both labelled **Office Hours**:

**Agenda issues:** Created by the moderator before each meeting using the **Meeting Agenda** template. Title format: `Office Hours Agenda: [DATE]`. The meeting notes are posted as a comment on this issue after the meeting, and the issue is closed once the recap blog post is published.

**Action item issues:** Created after each meeting for every action item identified during the session. These are task issues assigned to a responsible team member. Unlike content development issues, they relate to team process and coordination rather than learning content.

**Triage note:** Issues labelled **Office Hours** do not belong on any content project board (Topic Vetting, Content Development, Content Localization, Content Feedback). They are self-managed through the Office Hours workflow. If a triage member encounters an issue with this label, no further assignment to a content project board is needed.

For the full Office Hours workflow, see: [Organizing Office Hours Meetings](https://make.wordpress.org/training/handbook/training-team-how-to-guides/organizing-office-hours-meetings/)

---

---

## 4. GitHub Labels *(new page proposal)*

**Proposed URL:** https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/github-labels/

> **Note:** This page does not yet exist in the Make WordPress Training Handbook. This section proposes its creation, not a change to an existing page.

### Current situation

No dedicated handbook page for GitHub labels in the `WordPress/Learn` repository currently exists. The main *How We Use GitHub* page references labels in passing but does not document the label system, naming conventions, or individual labels in a structured way.

### Why this page is needed

The `WordPress/Learn` repository uses a structured label system with a `[Category]` prefix convention (e.g. `[Admin]`, `[Content]`, `[Localization]`). With the introduction of Office Hours, a new **Office Hours** label has been added. Without a dedicated labels page:
- Triage members have no reference for which labels exist and when to apply them
- Naming conventions (format, colour, purpose) are not documented
- New moderators and contributors cannot quickly understand the label structure

### Proposed new page

Create a new handbook sub-page *GitHub Labels* under *How We Use GitHub*, at the URL above. The page should document all active labels in the repository.

**Office Hours label:** suggested entry for the new page:

| Label | Category | Purpose |
|-------|----------|---------|
| `Office Hours` (or `[Admin] Office Hours`) | Admin | Marks all issues originating from the monthly Office Hours video meeting: agenda issues and action item issues. Not for content project boards. |

**Open question on naming convention:** Does the Office Hours label follow the existing `[Category]` prefix system? If so, it should be called `[Admin] Office Hours` rather than just `Office Hours`. This should be clarified within the team before the page is created.

**Scope note:** Documenting the Office Hours label is the immediate trigger for this proposal. The page would be most useful if it covers all labels in the repository, not just the Office Hours label.

---

## 5. Automated Workflows *(newly identified)*

**URL:** https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/automated-workflows/

### What the page currently covers

This page describes the automated GitHub workflows for the `WordPress/Learn` repository. Workflows automatically assign issues to project boards when they are created using an issue template.

### Problem

If the **Meeting Agenda** template is used (as it is for Office Hours agendas), an automated workflow could assign the issue to the wrong project board, for example an Admin board intended for regular meeting agendas, but not for Office Hours agendas.

The same risk applies to action item issues: depending on which template is used, they could be automatically assigned to content boards.

### Proposed change

**Check** whether the workflow for the Meeting Agenda template handles Office Hours issues correctly:

1. **Is the Office Hours label recognised?** If so, a workflow step can explicitly exclude Office Hours issues from content boards, or assign them to a dedicated board.
2. **Behaviour without a template:** If an Office Hours issue is created without a template, it falls into the general triage flow. The triage note on the *How We Use GitHub* main page and the label documentation are the main safeguards here.

If the workflow is adjusted, add a note to the Automated Workflows page:

> **Office Hours issues** (labelled `Office Hours`): If created via the Meeting Agenda template, these issues are not assigned to any content project board. The Office Hours label acts as a triage signal to exclude them from content development workflows.

---

## 6. Triaging Content Development Issues

**URL:** https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/triaging-content-development-issues/

### What the page currently covers

Step-by-step guide for the triage process of the Content Development project board. Issues pass through 5 status columns. Triage can be performed by Admins and Reps.

### Problem

Triage members working through the Content Development board could encounter Office Hours issues, for example if an action item issue was accidentally created without the correct label or template. Without a note, they might assign these issues to the content board or apply incorrect labels.

### Proposed change

Add a short note at the top of the page or in the introductory section:

> **Note:** Issues labelled **Office Hours** are not content development issues and should not be added to this project board. They originate from the team's monthly Office Hours video meetings and are managed through a separate workflow. See [Office Hours Issues](https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/#office-hours-issues) for details.

---

## 7. Validating and Applying Content Feedback

**URL:** https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/validating-and-applying-content-feedback/

### What the page currently covers

A two-part guide for validating and applying content feedback issues: one set of steps for validators, one for contributors applying the feedback.

### Problem

Office Hours meetings can produce feedback-related action items (e.g. "Review feedback on Course X and apply it"). These are created as Office Hours issues and are not regular content feedback issues. Without a note, triage members might assign them to the content feedback board.

### Proposed change

Add a short note at the top of the page (same wording as the other triage pages):

> **Note:** Issues labelled **Office Hours** are not content feedback issues and should not be added to this project board. They originate from the team's monthly Office Hours video meetings and are managed through a separate workflow. See [Office Hours Issues](https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/#office-hours-issues) for details.

---

## 8. Triaging Content Localization Issues

**URL:** https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/triaging-content-localization-issues/

### What the page currently covers

Triage guide for the Content Localization project board. Contributors open translation issues using the "Content Translation" template.

### Problem

Same situation as the other triage pages: Office Hours issues could accidentally be assigned to this board.

### Proposed change

Add the same short note as on the other triage pages:

> **Note:** Issues labelled **Office Hours** are not content localization issues and should not be added to this project board. They originate from the team's monthly Office Hours video meetings and are managed through a separate workflow. See [Office Hours Issues](https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/#office-hours-issues) for details.

---

## 9. Guidelines for Reviewing Content

**URL:** https://make.wordpress.org/training/handbook/training-team-how-to-guides/guidelines-for-reviewing-content-on-learn/

### What the page currently covers

Criteria and checklists for reviewing learning content (tutorials, courses) on Learn WordPress, both before and after publication.

### Problem

Office Hours meetings can generate content review action items. Someone receiving such a task via a GitHub issue should know that the review criteria on this page apply. This connection is not currently documented.

### Proposed change

A small, optional note at the top of the page:

> **How review tasks get assigned:** Content review tasks are sometimes assigned during the team's monthly [Office Hours meetings](https://make.wordpress.org/training/handbook/training-team-how-to-guides/organizing-office-hours-meetings/). If you received a review task via a GitHub issue labelled **Office Hours**, the same review guidelines on this page apply.

---

## 10. New GitHub Project Board *(new infrastructure)*

**URL (target location):** https://github.com/WordPress/Learn/projects?query=is%3Aopen

**URL (current personal board):** https://github.com/users/rfluethi/projects/10

### What currently exists

Topic proposals and the overview of Office Hours action items are currently tracked on a personal GitHub Project board (`github.com/users/rfluethi/projects/10`). This board is not part of the official Training Team infrastructure. It is not linked from the `WordPress/Learn` repository, and its visibility and long-term maintainability depend on a single person's account.

### Problem

A personal board is not a sustainable solution once Office Hours become an established team format. New contributors looking for open topics or ongoing tasks have no obvious place to look. Moderators planning a session cannot point to an official overview. There is also no consistent place to submit new topic proposals for contributors who are not yet familiar with the pilot repository (`github.com/rfluethi/wpt-office-hours`).

### Proposed action

Create a new GitHub Project under `https://github.com/WordPress/Learn/projects` specifically for Office Hours. The project should consolidate:

- **All agenda issues:** one card per upcoming and past meeting, giving a clear session history
- **All action item issues:** labelled `Office Hours`, tracking open tasks with owner and status
- **Topic proposals:** currently managed in the pilot repository; migrating them here makes the submission process accessible to all Training Team contributors directly within the main repository

The project board should use a simple Kanban structure with columns such as: *Proposed*, *Planned for Next Meeting*, *In Progress*, *Done*.

### Associated handbook change

Once the project board exists, add a reference to it in the *How We Use GitHub* main page (see [Section 3](#3-how-we-use-github-main-page)):

> **Office Hours Project Board:** All Office Hours issues (agendas, action items, and topic proposals) are tracked on the [Office Hours Project Board](https://github.com/WordPress/Learn/projects). This is the central place to see what was discussed, what is being worked on, and what topics have been proposed for upcoming meetings.

Also add a reference in the [Organizing Office Hours Meetings](https://make.wordpress.org/training/handbook/training-team-how-to-guides/organizing-office-hours-meetings/) handbook page, in the section on creating action item issues.

---

## Summary: Priority of changes

| Page | Priority | Type of change |
|------|----------|---------------|
| Hosting Training Team Meetings | **High** | Coffee Hours transition note + new Office Hours section |
| How to Write Meeting Agendas and Recap Posts | **High** | New section for Office Hours agenda and recap (incl. 48h draft step) |
| How We Use GitHub (main page) | **High** | New "Office Hours Issues" section + expanded use case list |
| GitHub Labels *(new page)* | **High** | Create new handbook sub-page under *How We Use GitHub*; document all labels including the Office Hours label; clarify naming convention (`Office Hours` vs. `[Admin] Office Hours`) |
| Automated Workflows | **Medium** | Check whether workflows handle Office Hours issues correctly; add note if adjusted |
| Triaging Content Development Issues | **Medium** | Short note: Office Hours label does not belong on this board |
| Validating and Applying Content Feedback | **Medium** | Short note: Office Hours label does not belong on this board |
| Triaging Content Localization Issues | **Medium** | Short note: Office Hours label does not belong on this board |
| Guidelines for Reviewing Content | **Low** | Optional cross-reference for contributors arriving via an Office Hours issue |
| New GitHub Project Board *(new infrastructure)* | **High** | Create official project board under WordPress/Learn; migrate topic proposals and action items from personal board; document in handbook |

---

*Sources: [Hosting Training Team Meetings](https://make.wordpress.org/training/handbook/training-team-how-to-guides/hosting-training-team-meetings/) · [How to Write Meeting Agendas](https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-to-write-a-meeting-agenda-or-recap/) · [How We Use GitHub](https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/) · [GitHub Labels](https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/github-labels/) · [Automated Workflows](https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/automated-workflows/) · [Triaging Content Development Issues](https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/triaging-content-development-issues/) · [Validating and Applying Content Feedback](https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/validating-and-applying-content-feedback/) · [Triaging Content Localization Issues](https://make.wordpress.org/training/handbook/training-team-how-to-guides/how-we-use-github/triaging-content-localization-issues/) · [Guidelines for Reviewing Content](https://make.wordpress.org/training/handbook/training-team-how-to-guides/guidelines-for-reviewing-content-on-learn/)*
