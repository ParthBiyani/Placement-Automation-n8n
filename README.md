PlacementPilot — n8n Workflows
================================

Introduction
-
PlacementPilot collects and surfaces job opportunities and related notifications for students and early-career job-seekers. These three n8n workflows automate discovery, notification, calendar scheduling, and LinkedIn outreach monitoring so students spend less time hunting and more time applying.

Problems faced by students
-
- Job postings are scattered across sites and hard to track.
- Students miss timely listings or forget to add interviews to calendars.
- Manual outreach on LinkedIn is repetitive and easy to miss.

Solution overview
-
- Combine three focused n8n workflows to: discover job posts, notify students instantly, create calendar events, and automate LinkedIn HR monitoring/outreach.
- Ready-to-import JSON files and screenshots show node layouts and required configuration.

Workflows
-

Find Jobs Automation
- Purpose: crawl or ingest job listings and compile a clean feed students can review.
- Student benefit: a consolidated list of curated roles, filtered and deduplicated.
- How it works: fetch → parse → filter → store or dispatch (e.g., sheet, DB, webhook).
- JSON: [workflows/Find Jobs Automation.json](workflows/Find%20Jobs%20Automation.json)

![Find Jobs Automation](workflow-screenshots/Find%20Jobs%20Automation.jpeg)


Job Listing Notifier and Calendar Event Set
- Purpose: send notifications for new job listings and create calendar events for application/interview reminders.
- Student benefit: immediate alerts and scheduled reminders so no deadlines slip.
- How it works: detect new listing → notify (email/Slack/WhatsApp) → create calendar event with details.
- JSON: [workflows/Job Listing Notifier and Calendar Event Set.json](workflows/Job%20Listing%20Notifier%20and%20Calendar%20Event%20Set.json)

![Job Listing Notifier and Calendar Event Set](workflow-screenshots/Job%20Listing%20Notifier%20and%20Calendar%20Event%20Set.jpeg)


LinkedIn HR Automation
- Purpose: monitor LinkedIn activity relevant to recruiting, then automate outreach or logging.
- Student benefit: timely follow-ups and automated messages/helpful reminders for networking.
- How it works: poll/monitor LinkedIn → filter relevant HR posts/messages → trigger outreach or record activity.
- JSON: [workflows/LinkedIn HR Automation.json](workflows/LinkedIn%20HR%20Automation.json)

![LinkedIn HR Automation](workflow-screenshots/LinkedIn%20HR%20Automation.jpeg)


Quick start (import)
- Open n8n and choose "Import" → point to the JSON file from the `workflows/` folder.
- Configure credentials (APIs, Gmail/Calendar, Slack, LinkedIn scraping or API) before activating.
- Test with one sample record and enable the workflow once verified.

Notes
- Replace placeholder credentials and API keys before enabling workflows.
- Adjust filters and schedules to match your campus timezone and preferred cadence.

License
- MIT-style: reuse freely; attribution appreciated.
