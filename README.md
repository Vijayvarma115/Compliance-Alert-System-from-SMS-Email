# Problem Statement

Businesses often miss compliance-related actions (like tax filings, returns, etc.) due to unnoticed email or SMS notifications. This leads to penalties and late fees.

# Solution 

Built an automation workflow that analyzes emails, detects compliance-related messages using regex, and then sends alerts, creates calendar reminders, and logs them into Notion.

# Automated Communication Workflow using n8n

This project showcases an automated end-to-end communication workflow built using **n8n**, aimed at reducing manual effort in managing incoming emails and scheduling events.

## 🚀 Features

- 🔔 **Email Trigger** via Gmail for real-time automation.
- 📤 **Conditional Logic** to route different types of messages.
- 💬 **Twilio SMS & Voice Alerts** for important emails.
- 📅 **Google Calendar Integration** to auto-create event entries.
- 📝 **Notion Integration** to log email content for future reference.

## 📷 Workflow Preview

![image](https://github.com/user-attachments/assets/e75ae133-a03d-4b38-8bb8-7a726549614e)

   # OverView Of n8n Workflow For BETTER Understanding

      𝗚𝗺𝗮𝗶𝗹 𝗡𝗼𝗱𝗲: Monitors all upcoming mails.

      𝗖𝗼𝗱𝗲 𝗡𝗼𝗱𝗲: Write logic(js)containing compliance-related keywords(eg:Duedate,penalty).

      𝗜𝗳 𝗡𝗼𝗱𝗲: Check if compliance-related keywords present if YES --->path1 else path2(useLess).

      𝗧𝘄𝗶𝗹𝗶𝗼 𝗡𝗼𝗱𝗲: Sends WhatsApp alert using Twilio(AuthSID,token).

      𝗖𝗼𝗱𝗲 𝗡𝗼𝗱𝗲: Extracts due date, amount, and penalty from the email(body/subject).

      𝗚𝗼𝗼𝗴𝗹𝗲 𝗖𝗮𝗹𝗲𝗻𝗱𝗮𝗿 𝗡𝗼𝗱𝗲: Creates the event on Calendar accordingly and make event 1day,2day,3day back before DueDate.

      𝗧𝘄𝗶𝗹𝗶𝗼 𝗡𝗼𝗱𝗲: Makes an Outbound call to the Customer regarding DueDate and Subject.

      𝗡𝗼𝘁𝗶𝗼𝗻 𝗡𝗼𝗱𝗲: Logs the compliance data .


## Notion Output

![image](https://github.com/user-attachments/assets/d90d0651-b60e-43c5-9d5d-ca69745ff2a3)


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




