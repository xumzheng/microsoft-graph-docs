---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	IssuingAuthority = "International Association of Branding Management"
	ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
}

Update-MgBetaUserProfileAward -UserId $userId -PersonAwardId $personAwardId -BodyParameter $params

```