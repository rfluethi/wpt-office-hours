# Organizing Office Hours Meetings

> **Status:** Draft, based on the [Office Hours proposal](https://make.wordpress.org/training/2026/02/03/proposal-monthly-office-hour-meeting-for-make-wordpress-training/) and decisions made at the [first Office Hours meeting (April 18, 2026)](https://github.com/WordPress/Learn/issues/3413).
>
> This guide covers the full process for organizing a Training Team Office Hours meeting: planning, running the meeting, creating GitHub issues for action items, and publishing the meeting notes.

---

## In this article

- [Overview](#overview)
- [1. Planning the Meeting](#1-planning-the-meeting)
  - [Confirm the date and moderator](#confirm-the-date-and-moderator)
  - [Confirm the note-taker](#confirm-the-note-taker)
  - [Set up Zoom](#set-up-zoom)
  - [Select the meeting topic and create the agenda](#select-the-meeting-topic-and-create-the-agenda)
  - [Announce the meeting](#announce-the-meeting)
- [2. Running the Meeting](#2-running-the-meeting)
  - [Before the call starts](#before-the-call-starts)
  - [Meeting structure](#meeting-structure)
  - [After the call ends](#after-the-call-ends)
- [3. Creating GitHub Issues for Action Items](#3-creating-github-issues-for-action-items)
- [4. Publishing the Meeting Notes](#4-publishing-the-meeting-notes)
  - [Step 1: Write the draft in the agenda issue](#step-1-write-the-draft-in-the-agenda-issue)
  - [Step 2: Allow time for corrections](#step-2-allow-time-for-corrections)
  - [Step 3: Publish on the Make WordPress Training blog](#step-3-publish-on-the-make-wordpress-training-blog)
  - [Step 4: Close the loop](#step-4-close-the-loop)
- [Moderation and note-taking rotation](#moderation-and-note-taking-rotation)
- [If things go wrong](#if-things-go-wrong)

---

## Overview

The Training Team Office Hours is a monthly 60-minute video meeting on Zoom. It is informal in tone but outcome-oriented: every meeting produces concrete action items, tracked as GitHub issues. Moderation and note-taking rotate among team members.

**Key repositories and links:**

| Resource | URL |
|----------|-----|
| Topic proposals (pilot phase) | [github.com/rfluethi/wpt-office-hours/issues](https://github.com/rfluethi/wpt-office-hours/issues) |
| Agenda issues & action item issues | [github.com/WordPress/Learn/issues](https://github.com/WordPress/Learn/issues) |
| New issue form | [github.com/WordPress/Learn/issues/new/choose](https://github.com/WordPress/Learn/issues/new/choose) |
| Meeting notes published on | [make.wordpress.org/training](https://make.wordpress.org/training/) |
| Agenda template (reference) | [`/templates/agenda.md`](../templates/agenda.md) |
| Meeting notes template (reference) | [`/templates/meeting-notes.md`](../templates/meeting-notes.md) |
| Slack channel | [`#training`](https://wordpress.slack.com/archives/C02RW657Q) |

---

## 1. Planning the Meeting

Planning should begin **at least two weeks** before the meeting. The previous meeting's final agenda item is to confirm the date, moderator, and note-taker for the next meeting; use those decisions as your starting point.

### Confirm the date and moderator

The date and moderator for the next meeting are decided at the end of each Office Hours session and recorded in the meeting notes. Before planning begins, confirm that both are still available.

**Scheduling guidelines:**
- Meetings are held once per month, typically on a **Saturday at 14:00 UTC**.
- The time slot may rotate across meetings to accommodate different time zones.
- Consult any published polls on preferred meeting times (see action items from previous meetings).
- Avoid dates that conflict with major WordPress events (WordCamps, contributor days) or public holidays in participants' regions.

**Moderator responsibilities:**
- Any Training Team member may moderate.
- No one should moderate more than once every three months.
- The moderator is supported by a co-moderator (the note-taker or another participant willing to step in if needed).
- If you are moderating for the first time, reach out to a previous moderator for a brief prep conversation.
- At least one **Team Representative** should be present at each meeting to ensure overall coordination.

### Confirm the note-taker

The note-taker is responsible for writing up the meeting notes after the meeting. If no note-taker was confirmed at the previous meeting, ask for a volunteer in the `#training` Slack channel. No one should take notes more than once every three months.

### Set up Zoom

The Training Team uses the shared team Zoom account for Office Hours. If you need access to the shared Zoom account, request it in advance by pinging `@tt-admins` in the `#training` channel.

Steps:
1. Create a Zoom meeting for the confirmed date and time.
2. Set the duration to 60 minutes.
3. Enable the waiting room (optional, to control who enters).
4. Copy the Zoom link; you will need it for the agenda and all announcements.
5. Test audio and screen sharing before the meeting day.

### Select the meeting topic and create the agenda

**Selecting the topic:**

Topic proposals are collected as GitHub issues in the [wpt-office-hours repository](https://github.com/rfluethi/wpt-office-hours/issues). The moderator reviews open proposals and selects the topic for the upcoming meeting. When selecting a topic, consider:
- Topics that have been waiting longest
- Topics that have high community interest (upvotes, comments)
- Topics that require a decision from the team

**Creating the agenda:**

The agenda is published as a new GitHub issue in the main Training Team repository. Use the [agenda template](../templates/agenda.md) as a structural reference.

1. Go to [github.com/WordPress/Learn/issues/new/choose](https://github.com/WordPress/Learn/issues/new/choose) and select the **Meeting Agenda** template.
2. Set the issue title to: `Office Hours Agenda: [DATE]` (e.g. `Office Hours Agenda: May 23, 2026`).
3. Fill in all placeholders in the issue body: date, time, Zoom link, moderator, note-taker, discussion topic, and discussion questions.
4. Apply the **Office Hours** label.
5. **Publish the agenda at least 48 hours before the meeting** so that participants, especially non-native English speakers, have time to prepare.

> **Why this matters:** Announcing the topic in advance is a deliberate accessibility measure. It gives participants time to read background material and prepare their thoughts in English.

### Announce the meeting

**Slack `#training` channel**

Send two reminders in the `#training` channel:
- **One week before:** Share the agenda issue link, meeting date, time, and Zoom link.
- **24 hours before:** Short reminder with date, time, Zoom link, and agenda link.

Also add the meeting to the [Make WordPress meetings calendar](https://make.wordpress.org/meetings/#training) if you have access, or ask a Team Rep to do so.

---

## 2. Running the Meeting

### Before the call starts

- Open the Zoom meeting a few minutes early to greet early arrivals.
- Post the Slack opening tag in `#training` with the Zoom link:

  ```
  <office hour meeting> Office Hours starting now! Join us: [ZOOM LINK]
  ```

  > **Why this tag matters:** The `<office hour meeting>` tag is recognized by the Make WordPress Slack bot, which logs the meeting duration for [Five for the Future](https://make.wordpress.org/five-for-the-future/) contributor tracking. All participants' time is officially recorded as a WordPress contribution. Do not skip this step.

- Have the agenda issue open and ready to share.
- Share the agenda link in the Zoom chat as participants join.

### Meeting structure

The Office Hours follow a fixed structure. Keep an eye on the time and move sections along as needed.

| Time | Section | Duration |
|------|---------|---------|
| 00:00–05:00 | **Welcome & Onboarding** | 5 min |
| 05:00–15:00 | **Brief Introductions** | 10 min |
| 15:00–25:00 | **Topic Presentation** | 10 min |
| 25:00–50:00 | **Open Discussion** | 25 min |
| 50:00–60:00 | **Review, Next Steps & Wrap-Up** | 10 min |

**Welcome & Onboarding (5 min)**
- Welcome participants and remind them of the [WordPress Community Code of Conduct](https://make.wordpress.org/handbook/community-code-of-conduct/).
- Ask if anyone has accessibility needs the group should be aware of.
- Note the WordPress.org usernames of everyone present (the note-taker will need them).

**Brief Introductions (10 min)**
- Ask each participant for a brief introduction: name, location, role in the WordPress ecosystem.
- For repeat participants, keep this short. Prioritize new faces.

**Topic Presentation (10 min)**
- Briefly introduce the meeting's main topic: what it is, why it matters, what the group hopes to decide or achieve.
- If a presentation or background material was prepared, share it now (max. 10 minutes).
- The goal is to bring everyone to the same level of understanding before the discussion opens.

**Open Discussion (25 min)**
- Work through the discussion questions listed in the agenda.
- The moderator's role is to facilitate, not to decide. Seek consensus; if consensus is not possible, document the different viewpoints and note that a decision needs to be escalated to Team Reps.
- Keep the discussion outcome-oriented. If a topic needs more time than available, note it as an open question and propose a follow-up (a smaller group, an async discussion, or a future meeting topic).
- Watch for participants who haven't spoken yet and invite them in.

**Review, Next Steps & Wrap-Up (10 min)**

Work through the following items in order:

1. **Review of open action items from previous meetings:** Ask responsible persons for a brief status update. If something is blocked or delayed, document it. This is a short checkpoint, not a full re-discussion.
2. **Definition of next steps:** Summarize the decisions made and confirm each action item: task description, responsible person, and target date (where possible).
3. **Set the date, moderator, and note-taker for the next meeting:** Confirm these with the group before closing.
4. **Wrap-up:** Thank all participants. Remind them that meeting notes will be posted as a comment on this agenda issue within approximately 48 hours and that corrections are welcome.

### After the call ends

Immediately after the meeting ends:

1. Post the Slack closing tag in `#training`:

   ```
   </office hour meeting> Thanks everyone for joining! Notes coming within 48h.
   ```

2. Share a brief summary of decisions and action items in the `#training` Slack thread.
3. Ensure the next meeting is listed on the [Make WordPress Training homepage](https://make.wordpress.org/training/). If needed, create a GitHub issue and assign it to the next moderator to take care of this.

---

## 3. Creating GitHub Issues for Action Items

All action items from the Office Hours are tracked as issues in the main Training Team repository, not in the pilot repository. This ensures Office Hours tasks are part of the team's regular workflow and visible to everyone.

**Repository:** [github.com/WordPress/Learn/issues](https://github.com/WordPress/Learn/issues)
**New issue form:** [github.com/WordPress/Learn/issues/new/choose](https://github.com/WordPress/Learn/issues/new/choose)

**Steps for each action item:**

1. Go to the [new issue form](https://github.com/WordPress/Learn/issues/new/choose) and select the most appropriate issue template.
2. Set the issue title to a clear, actionable description of the task (e.g. "Create and publish Office Hours meeting notes").
3. In the issue body, include:
   - A brief description of the task
   - The name and WordPress.org username of the responsible person
   - The target completion date (if applicable)
   - A reference back to the meeting where the task was created (link to the agenda issue)
4. Apply the **Office Hours** label to the issue. This label distinguishes Office Hours tasks from the broader Training Team backlog.
5. Assign the issue to the responsible person if they have a GitHub account.
6. Record the issue number in the meeting notes action items table.

**Tracking and follow-up:**

- Open action items are reviewed at the beginning of each subsequent Office Hours as a standing agenda item.
- If a responsible person cannot complete a task, they should communicate this proactively in the `#training` Slack channel or in a comment on the issue; do not leave issues silently open.
- When a task is completed, close the GitHub issue.

---

## 4. Publishing the Meeting Notes

The note-taker is responsible for writing up and publishing the meeting notes. The process has four steps.

### Step 1: Write the draft in the agenda issue

The meeting notes are written as a comment on the agenda GitHub issue, not as a separate file.

1. Open the agenda issue for this meeting in [github.com/WordPress/Learn/issues](https://github.com/WordPress/Learn/issues).
2. Use the [meeting notes template](../templates/meeting-notes.md) as a structural guide for the comment.
3. Fill in all sections:
   - **Meeting Context:** 2–4 sentences explaining what this meeting was about and why it matters.
   - **Participants:** Full names and WordPress.org usernames (not Slack usernames). Use the table format from the template.
   - **Topics Discussed:** For each topic: a narrative discussion summary (who said what and why it mattered) and a scannable outcome bullet list.
   - **Decisions:** Only formal decisions, listed in the decisions table. Add a rationale note for any decision where the reasoning is important to preserve.
   - **Action Items:** Every action item with task description, responsible person (WordPress.org username), and status. Link to the corresponding GitHub issue number.
   - **Follow-up from Previous Meeting:** Status of action items from the previous meeting.
   - **Next Meeting:** Date, time, moderator, and proposed topics.
4. Post the comment as a draft note and share the link to the issue in the `#training` Slack channel so participants know where to submit corrections.

> **Note on WordPress.org usernames:** Always use WordPress.org usernames (e.g. `@rfluethi`), not Slack display names. If you are unsure of someone's WordPress.org username, open their Slack profile, copy their Slack member ID, and open `https://profiles.wordpress.org/SLACK_USER_ID/`, which will redirect to their WordPress.org profile.

### Step 2: Allow time for corrections

- Leave the draft open for corrections for approximately **48 hours** after the meeting.
- Participants can suggest corrections by commenting on the issue.
- The note-taker reviews feedback and incorporates any factual corrections.

### Step 3: Publish on the Make WordPress Training blog

1. Go to [make.wordpress.org/training/wp-admin](https://make.wordpress.org/training/wp-admin) and log in with your WordPress.org account.
   - If you do not have Author access, ask a Training Team admin: ping `@tt-admins` in the `#training` channel.
   - Example message: *"Hi @tt-admins. I am the note-taker for the Office Hours meeting on [DATE]. Please grant me Author access to make.wordpress.org/training. Thanks!"*
2. Select **Post > Add New** from the left sidebar.
3. Use the **Recap for Training Team Meeting** pattern as a structural starting point (type `/recap` in the post editor to activate it), but adapt it to the Office Hours format; the content will be richer than a standard Slack meeting recap.
4. Include in the published post:
   - Meeting date, time, platform, moderator, note-taker
   - Link to the meeting agenda (GitHub issue)
   - List of participants (WordPress.org usernames)
   - Summary of topics discussed and decisions made
   - Full action items table with GitHub issue links
   - Next meeting date and moderator
5. Add the appropriate **categories** and **tags**. At minimum:
   - Category: `Meeting Recap`
   - Tags: `office-hours`, `training`, `meeting-recap`
6. If you include any images, add alt text to every image.
7. **Do not paste Google Docs or Google Spreadsheet links** in the post. Link to Slack messages or GitHub issues instead.
8. Save as a draft and ping `@tt-admins` in the `#training` channel with a link to the draft for review.
   - Example message: *"Hi @tt-admins. The Office Hours recap for [DATE] is ready for review: [DRAFT LINK]. Please publish once confirmed. Thanks!"*
9. A team admin will review and publish the post.

### Step 4: Close the loop

Once the post is published:

1. Add a comment to the agenda GitHub issue with a link to the published blog post.
2. Close the agenda issue.
3. Post the blog post link in the `#training` Slack channel.

---

## Moderation and note-taking rotation

Moderation and note-taking both rotate among team members. The guidelines below apply equally to both roles and help keep the rotation fair and sustainable.

- **No one should moderate or take notes more than once every three months.**
- The next meeting's moderator and note-taker are confirmed at the end of each meeting and recorded in the meeting notes.
- Any Training Team member may take on either role; experience is not required, and support is available.
- **First-time moderators** are encouraged to reach out to a previous moderator for a brief prep call. The agenda checklist and this guide are your main preparation tools.
- Both the moderator and the note-taker have the right to decline without explanation. If a confirmed person needs to step down, they should notify the group at least one week in advance so a replacement can be found.
- The **co-moderator** (typically the note-taker or another willing participant) is available as backup. If both moderator and co-moderator are unavailable, the meeting is rescheduled with at least 48 hours' notice.

---

## If things go wrong

**Low attendance (fewer than 3 participants)**
- Convert the session to an async discussion in the `#training` Slack channel.
- Post a summary of the agenda topic and ask for responses asynchronously.
- Do not count this session towards the pilot phase metrics.

**Moderator unavailable (less than 48h notice)**
- The co-moderator takes over.
- If both are unavailable, post a cancellation notice in `#training` and reschedule within the same month if possible.

**Technical issues (Zoom problems)**
- Switch to an alternative platform if identified in advance (Jitsi is the evaluated fallback).
- If no alternative is available, continue the meeting as a Slack text discussion in `#training`.
- Always close with the `</office hour meeting>` tag, even if the meeting moved platforms.

**Code of Conduct issues**
- The moderator may pause or end the meeting.
- A Team Representative handles follow-up according to the [WordPress Community Code of Conduct](https://make.wordpress.org/handbook/community-code-of-conduct/).

---

*This guide was drafted based on the [Office Hours proposal](https://make.wordpress.org/training/2026/02/03/proposal-monthly-office-hour-meeting-for-make-wordpress-training/) and the decisions made at the first Office Hours meeting on April 18, 2026. For questions, post in the [`#training`](https://wordpress.slack.com/archives/C02RW657Q) Slack channel.*
