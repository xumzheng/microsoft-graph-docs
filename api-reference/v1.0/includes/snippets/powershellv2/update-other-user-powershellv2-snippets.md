---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Users

$params = @{
	businessPhones = @(
		"+1 425 555 0109"
	)
	officeLocation = "18/2111"
}

Update-MgUser -UserId $userId -BodyParameter $params

```