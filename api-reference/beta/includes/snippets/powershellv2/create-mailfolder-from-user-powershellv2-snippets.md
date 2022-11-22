---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Mail

$params = @{
	DisplayName = "Clutter"
	IsHidden = $true
}

# A UPN can also be used as -UserId.
New-MgBetaUserMailFolder -UserId $userId -BodyParameter $params

```