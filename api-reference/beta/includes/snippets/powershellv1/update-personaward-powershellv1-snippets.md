---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.People

$params = @{
	IssuingAuthority = "International Association of Branding Management"
	ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
}

Update-MgUserProfileAward -UserId $userId -PersonAwardId $personAwardId -BodyParameter $params

```