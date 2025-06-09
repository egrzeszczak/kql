# kql

A collection of my KQL queries

## **Detection rules (Microsoft Defender XDR)**
|Name|Description|MITRE ATT&CK
|-|-|-|
|[Email forwarding to external domain](./detection-rules/Email-forwarding-to-external-domain/query.kql)|Detects creation of mailbox rules that have ForwardTo, ForwardAsAttachmentTo, or RedirectTo set to an external, untrusted domain (in Outlook Web). You specify trusted domains in the query.|T1114: Email Collection, T1114.003: Email Forwarding Rule|
|[Email forwarding to external domain (Classic)](./detection-rules/Email-forwarding-to-external-domain-\(Classic\)/query.kql)|Detects creation of mailbox rules that have ForwardTo, ForwardAsAttachmentTo, or RedirectTo set to an external, untrusted domain (in Outlook Classic). You specify trusted domains in the query.|T1114: Email Collection, T1114.003: Email Forwarding Rule|
|[Email sent via forwarding to external domain](./detection-rules/Email-sent-via-forwarding-to-external-domain/query.kql)|Detects email messages that were forwarded to an external domain. You specify trusted domains in the query.|T1114: Email Collection, T1114.003: Email Forwarding Rule|
|[Trusted domain blocked by Defender](./detection-rules/Trusted-domain-blocked-by-Defender/query.kql)|Checks for web filtering blocks to trusted domains. You specify trusted domains in the query.|T1071: Application Layer Protocol, T1071.001: Web Protocols|
|[Failed Conditional Access action](./detection-rules/Failed-Conditional-Access-action/query.kql)|Detects failed Conditional Access actions for a specified rule ID has been detected. You set the RuleID in the query.|T1556.009: Conditional Access Policies|