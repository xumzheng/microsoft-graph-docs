---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessage -UserId $userId -Filter "MentionsPreview/IsMentioned eq true" -Property "Subject,Sender,ReceivedDateTime,MentionsPreview" 

```