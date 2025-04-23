# Automated Communication Workflow using n8n

This project showcases an automated end-to-end communication workflow built using **n8n**, aimed at reducing manual effort in managing incoming emails and scheduling events. It was developed during my internship to streamline notifications and record-keeping across different platforms.

## 🚀 Features

- 🔔 **Email Trigger** via Gmail for real-time automation.
- 📤 **Conditional Logic** to route different types of messages.
- 💬 **Twilio SMS & Voice Alerts** for important emails.
- 📅 **Google Calendar Integration** to auto-create event entries.
- 📝 **Notion Integration** to log email content for future reference.

## 🔧 Tech Stack

- [n8n](https://n8n.io/) – Workflow automation
- [Gmail API](https://developers.google.com/gmail/api)
- [Twilio](https://www.twilio.com/) – SMS & voice call service
- [Google Calendar API](https://developers.google.com/calendar)
- [Notion API](https://developers.notion.com/) – Database page creation

## 📌 Use Case

This workflow is ideal for:
- Teams that need to be notified immediately when priority emails arrive.
- Automatically creating reminders/events based on email content.
- Logging key communications into Notion for documentation.

## 🛠️ Setup

1. Clone the repo or import the workflow JSON into your n8n instance.
2. Connect the following accounts in n8n:
   - Gmail (for trigger)
   - Twilio (SMS & call)
   - Google Calendar
   - Notion
3. Update credentials and phone numbers in the workflow.
4. Activate the workflow.

## 📷 Workflow Preview

![Workflow Diagram](./workflow-preview.png)



