---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

# A UPN can also be used as -UserId.
Get-MgBetaUserMessage -UserId $userId -Filter "MentionsPreview/IsMentioned eq true" -Property "Subject,Sender,ReceivedDateTime,MentionsPreview" 

```