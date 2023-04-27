---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	displayName = "Business Email"
	type = "work"
}

Update-MgBetaUserProfileEmail -UserId $userId -ItemEmailId $itemEmailId -BodyParameter $params

```