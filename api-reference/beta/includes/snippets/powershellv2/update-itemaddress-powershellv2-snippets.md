---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	allowedAudiences = "me"
	displayName = "Secret Hideout"
}

Update-MgBetaUserProfileAddress -UserId $userId -ItemAddressId $itemAddressId -BodyParameter $params

```