# kql

A collection of my KQL queries

## **Detection rules (Microsoft Defender XDR)**
|Name|Description|MITRE ATT&CK
|-|-|-|
|[Email forwarding to external domain](./detection-rules/Email-forwarding-to-external-domain/query.kql)|Detects creation of mailbox rules that have ForwardTo, ForwardAsAttachmentTo, or RedirectTo set to an external, untrusted domain. You specify trusted domains in the query (Outlook Web)|T1114: Email Collection, T1114.003: Email Forwarding Rule|
|[Email forwarding to external domain (Classic)](./detection-rules/Email-forwarding-to-external-domain-\(Classic\)/query.kql)|Detects creation of mailbox rules that have ForwardTo, ForwardAsAttachmentTo, or RedirectTo set to an external, untrusted domain. You specify trusted domains in the query (Outlook Classic)|T1114: Email Collection, T1114.003: Email Forwarding Rule|