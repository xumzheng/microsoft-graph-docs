---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	AllowedAudiences = "me"
	DisplayName = "Secret Hideout"
}

Update-MgBetaUserProfileAddress -UserId $userId -ItemAddressId $itemAddressId -BodyParameter $params

```