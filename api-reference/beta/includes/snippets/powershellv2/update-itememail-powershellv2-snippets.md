---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	DisplayName = "Business Email"
	Type = "work"
}

Update-MgBetaUserProfileEmail -UserId $userId -ItemEmailId $itemEmailId -BodyParameter $params

```