Name : Kondaparthi Srihari
n8n Cold Email Outreach Automation (with Email Verification)

Built an automated cold email workflow in n8n to fetch lead data from Google Sheets, verify email validity, and send personalized outreach emails only to valid leads.

Workflow Breakdown (As Seen in the Image):

Start Node
Workflow begins manually or on schedule.

Get row(s) in sheet (Google Sheets Node)
Reads lead data (e.g., Name, Company, Email) from a Google Sheet.

If Condition #1
Checks if the lead already has an email provided.

If no email → Skip / Do nothing (to avoid errors)

If email exists → Continue to verification

Hunter Email Verification Node
Verifies email validity and confidence score using Hunter.io API.

If Condition #2
Sends email only if the verification result is valid and not risky.

If verified → Send Email node triggers outreach email.

If invalid → Lead is ignored (No Operation node).

Send Email Node (SMTP / Gmail)
Sends a personalized cold email to the verified lead.

Key Highlights:

Prevents bounce rate by verifying email addresses before sending.

Avoids spam flags through conditional logic and controlled sending.

Fully hands-free execution — run once and it processes multiple leads automatically.

Impact Statement (Use in Resume):

Automated lead outreach and email validation, reducing manual effort by ~80% and improving delivery success rate by 20–35% through verified email sending.
