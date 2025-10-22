# Automated-Invoice-Reminder-System
This workflow automatically sends invoice reminder emails based on the status of each invoice stored in Google Sheets. It helps companies follow up on pending payments without manual effort.
✅ Workflow Logic
Step	Node	Description
1	Manual Trigger	Starts the workflow (can be replaced with Cron for automation).
2	Google Sheets – Read Rows	Fetches all invoice data from the sheet.
3	Filter / IF (optional)	Organizes and filters invoice entries.
4	Switch Node	Routes invoices based on the Status column.
5	Gmail – Send Email	Sends reminders to customers or notifications to company.
📨 Email Rules
Invoice Status	Action	Recipient
Unpaid	Send Reminder Email	Customer
Overdue	Send Final Notice	Customer
Finished	Send Info Email (or skip)	Company
✉️ Email Types

Unpaid Reminder: Inform customer about pending invoice

Overdue Notice: Warn about late payment

Finished Notification: Notify company that invoice is paid

🛠️ Tools Used

n8n

Google Sheets

Gmail API

(Optional) Cron Trigger for auto scheduling

✅ Result

This workflow makes your invoice follow-up fully automated, saves time, and increases payment recovery efficiency.
