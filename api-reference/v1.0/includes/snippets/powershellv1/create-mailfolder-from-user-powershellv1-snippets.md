---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Mail

$params = @{
	DisplayName = "Clutter"
	IsHidden = $true
}

# A UPN can also be used as -UserId.
New-MgUserMailFolder -UserId $userId -BodyParameter $params

```