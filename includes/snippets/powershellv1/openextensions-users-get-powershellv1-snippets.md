---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUser -UserId $userId -Property "id,displayName,mail,mobilePhone" -ExpandProperty "extensions" 

```