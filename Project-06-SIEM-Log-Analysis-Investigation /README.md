## Incident Summary
A security event was reviewed following the identification of suspicious authentication behaviour within Microsoft Sentinel. The investigation focused on analysing sign-in activity to determine whether the observed behaviour indicated unauthorised access or aligned with normal user behaviour.

The objective was to understand what triggered the alert, assess the associated risk, and decide whether escalation or remediation actions were required.

## Detection / Alert Trigger
The investigation was initiated after Microsoft Sentinel highlighted a sign-in pattern involving multiple failed authentication attempts followed by a successful login for the same user account within a short period of time. This pattern can sometimes be associated with password guessing or compromised credentials and therefore required further review.

## Scope of Investigation
The investigation was limited to authentication-related telemetry ingested into Microsoft Sentinel. Analysis focused exclusively on identity sign-in events, including authentication outcomes, timestamps, source IP addresses, and location context. No endpoint, email, or mailbox data was included as part of this investigation.

## Log Source Overview
The analysis was based on identity authentication logs commonly ingested into Microsoft Sentinel through Azure Monitor and Log Analytics. These logs provide visibility into user sign-in behaviour, including success and failure results, originating IP addresses, geographic information, and event timing. This telemetry forms the primary data source for authentication investigations within Sentinel.

## Initial Log Review
An initial review of sign-in events was performed to identify patterns that could indicate suspicious behaviour. The review focused on identifying repeated failed authentication attempts, successful sign-ins occurring shortly after failures, and any indications of access from unfamiliar locations or IP addresses. The aim at this stage was to determine whether the activity was more consistent with credential misuse or typical user behaviour such as mistyped passwords.

## SIEM Analysis and Correlation
Further analysis was conducted by correlating multiple log attributes within Microsoft Sentinel. Sign-in events were reviewed together to assess the relationship between timestamps, IP addresses, locations, and authentication outcomes across the activity window. Correlating these fields helped determine whether the behaviour was isolated or suggestive of unauthorised access attempts.

This correlation approach allowed the investigation to move beyond individual events and assess the overall sign-in pattern in context.

## Investigation Findings
The investigation identified activity that warranted review; however, there was insufficient evidence to confirm unauthorised access. The successful sign-in aligned with expected location and access patterns for the user, and no additional suspicious authentication activity was observed during the review period. There were no indicators of abnormal locations, unfamiliar IP addresses, or escalation in sign-in behaviour following the successful authentication.

## Analyst Decision and Outcome
Based on the findings, no immediate response actions were required. The activity was assessed as low risk, and escalation or remediation actions such as credential resets or account restrictions were not initiated. Continued monitoring was recommended to ensure visibility of any recurring authentication anomalies.

## Incident Closure
The incident was closed after completing log review and correlation within Microsoft Sentinel. No further action was required beyond standard monitoring for similar authentication patterns in the future.

## Lessons Learned
Authentication patterns involving repeated failures followed by a successful login should always be reviewed in context. Microsoft Sentinel enables effective investigation by allowing analysts to correlate multiple authentication attributes, helping distinguish between normal user behaviour and potential security threats without unnecessary escalation.
