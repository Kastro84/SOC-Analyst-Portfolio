# Project 1 – Phishing → Identity Compromise Investigation

## Scenario Overview
A phishing email targeting a user mailbox was reviewed as part of a simulated SOC investigation. The message impersonated a legitimate service and contained a link intended to capture user credentials. The investigation focused on confirming whether the user interacted with the email and assessing whether any suspicious sign-in activity occurred after the message was received.
## Evidence Collected (Screenshots)

## Alert / Detection Trigger
The investigation was initiated after a phishing alert was raised for a suspicious sender domain and an embedded link commonly associated with credential harvesting. The email was flagged for review to assess potential user impact.
## Initial Triage – Email Analysis
Reviewed sender address and display name for impersonation indicators

Checked sender domain reputation and age

Analysed subject line and email body for urgency or social engineering tactics

Extracted and reviewed the embedded URL for redirection or credential harvesting behaviour

Confirmed whether the user interacted with the email or clicked the link

Checked if similar emails were delivered to other users
## Identity Investigation
Reviewed recent sign-in activity for the affected user account following receipt of the phishing email

Checked for sign-ins originating from unfamiliar locations, IP addresses, or devices

Looked for patterns of failed sign-in attempts followed by a successful authentication

Reviewed the authentication methods used during sign-ins, including whether MFA was prompted or bypassed

Checked for any high-risk or flagged sign-in events during the relevant timeframe

Verified whether any account changes or unusual activity occurred after the suspected phishing interaction
## Findings & Correlation
The email was confirmed to be phishing based on the sender details and the behaviour of the embedded link

There was no indication that the user interacted with the email or entered their credentials

Review of sign-in activity did not show any unusual or unexpected authentication attempts after the email was received

No account changes or other indicators of compromise were identified during the review period
## Response & Decision
The phishing email was removed from the user’s mailbox

The user was advised not to interact with similar emails going forward

A password reset was not required as there were no signs of account compromise

The account was monitored after the alert to ensure no delayed suspicious activity occurred
## Incident Closure
The incident was closed after confirming there was no user interaction or follow-on account activity
Reviewing phishing alerts quickly helps reduce the risk of credential compromise

Confirming user interaction and sign-in activity is important before taking disruptive actions

Clear communication with users helps prevent repeat incidents
No further action was required beyond user awareness and monitoring
## Notes / Lessons Learned
Reviewing phishing alerts quickly helps reduce the risk of credential compromise

Confirming user interaction and sign-in activity is important before taking disruptive actions

Clear communication with users helps prevent repeat incidents
