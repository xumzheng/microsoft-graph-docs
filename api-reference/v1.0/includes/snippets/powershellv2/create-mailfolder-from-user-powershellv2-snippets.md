---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Mail

$params = @{
	displayName = "Clutter"
	isHidden = $true
}

# A UPN can also be used as -UserId.
New-MgUserMailFolder -UserId $userId -BodyParameter $params

```