# Project 2 – MFA Fatigue / Suspicious Authentication Investigation

## Scenario Overview
Multiple authentication prompts were generated for a user account within a short period of time, prompting a review for potential MFA fatigue or unauthorized access attempts. The investigation focused on determining whether the activity reflected malicious behaviour or aligned with expected user authentication patterns.

## Environment & Evidence Context


## Alert / Detection Trigger
The review was initiated after a pattern of repeated authentication attempts was observed for a single user account within a short timeframe. The frequency and timing of the sign-in activity were inconsistent with typical user behaviour, prompting further investigation to assess the risk of MFA fatigue or unauthorized access.

## Initial Triage – Authentication Review
Initial triage focused on reviewing authentication activity associated with the affected user account. Sign-in logs were examined to understand the volume, timing, and outcome of authentication attempts, as well as whether the activity originated from expected locations and devices. Particular attention was given to identifying repeated MFA challenges, failed sign-in attempts, and any signs of abnormal authentication behaviour.

## Identity Investigation
The identity investigation focused on reviewing authentication behaviour in more detail to determine whether the activity suggested attempted account compromise. Sign-in logs were analysed to assess the consistency of locations, devices, and authentication methods used during the period of repeated MFA prompts.

MFA challenge outcomes were reviewed to confirm whether prompts were approved, denied, or left unanswered, and to identify whether any successful sign-ins followed the repeated authentication attempts. The investigation also considered whether the authentication activity aligned with the user’s normal sign-in patterns or indicated abnormal behaviour.

## Findings & Correlation
Review of the authentication activity showed repeated MFA prompts without evidence of successful unauthorized access. Sign-in attempts originated from expected locations and devices associated with the user account, and there were no unfamiliar IP addresses or authentication methods observed.

No sign-in events indicated elevated risk, and there were no account changes or follow-on activity suggesting credential compromise. The authentication behaviour was consistent with user-initiated sign-in attempts rather than an external MFA fatigue attack.

## Analyst Decision Points
Several response options were considered during the investigation. These included forcing a password reset, resetting MFA methods, or escalating the case for further review. Each option was weighed against the available evidence and the potential impact on the user.

Given the absence of successful unauthorized sign-ins, unfamiliar locations, or elevated risk indicators, disruptive actions were not taken. The decision was made to continue monitoring the account rather than apply immediate remediation.

## Response & Decision
No immediate remediation actions were taken, as the investigation did not identify evidence of account compromise or MFA abuse. The user account was monitored for further abnormal authentication activity, and guidance was provided to report any unexpected MFA prompts promptly.

Incident Severity: Low

## Incident Closure
The incident was closed after confirming that the authentication activity did not indicate MFA fatigue or unauthorized access. No further suspicious behaviour was observed following the initial review, and the account remained stable during the monitoring period.

## Notes / Lessons Learned
Repeated MFA prompts should be reviewed in context. When no compromise indicators are present, monitoring may be sufficient.

## Evidence Collected (Screenshots)


## What Would Have Changed the Outcome
The response would have escalated if there had been evidence of successful sign-ins from unfamiliar locations or devices, repeated MFA approvals following failed attempts, elevated sign-in risk indicators, or account changes occurring after the authentication activity.
