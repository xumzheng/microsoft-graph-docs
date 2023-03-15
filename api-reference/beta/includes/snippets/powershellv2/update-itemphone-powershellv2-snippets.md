---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Type = "other"
}

Update-MgBetaUserProfilePhone -UserId $userId -ItemPhoneId $itemPhoneId -BodyParameter $params

```