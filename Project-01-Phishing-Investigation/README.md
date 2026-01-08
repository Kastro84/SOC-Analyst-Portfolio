# Project 1 – Phishing → Identity Compromise Investigation

## Scenario Overview
A phishing email targeting a user mailbox was reviewed during a SOC-style investigation. The email impersonated a legitimate service and included a link intended to capture user credentials. The investigation focused on whether the user interacted with the email and whether any suspicious sign-in activity followed.

## Alert / Detection Trigger
The investigation started after a phishing alert was raised for an email containing a suspicious sender domain and embedded link. The alert required review to assess whether the email posed a risk to the user account.

## Initial Triage – Email Analysis
The email was reviewed for signs of impersonation and social engineering. The sender address, sender domain, subject line, and message content were checked for common phishing indicators. The embedded link was reviewed to determine whether it led to a credential harvesting page. It was also confirmed whether the user interacted with the email and whether similar messages were delivered to other users.

## Identity Investigation
The affected user’s sign-in activity was reviewed after the phishing email was received. Authentication logs were checked for unfamiliar locations, devices, or IP addresses. The review focused on identifying failed sign-in attempts, successful logins, MFA behaviour, and any flagged or high-risk sign-in events. Account activity was also checked for unexpected changes.

## Findings & Correlation
The email was confirmed to be phishing based on the sender details and link behaviour. There was no evidence the user interacted with the email or entered credentials. Sign-in activity did not show any unusual behaviour, and no indicators of account compromise were identified.

## Response & Decision
The phishing email was removed from the mailbox. The user was advised to remain cautious of similar messages. A password reset was not required, as there were no signs of compromise. The account was monitored to ensure no delayed suspicious activity occurred.

## Incident Closure
The incident was closed after confirming there was no user interaction with the phishing email and no related suspicious account activity. No further action was required beyond monitoring.

## Notes / Lessons Learned
Quick review of phishing alerts helps reduce risk. Confirming user interaction and checking sign-in activity is important before taking disruptive actions. Clear user communication supports better security awareness.
