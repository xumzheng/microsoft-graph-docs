---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Publisher = "International Association of Branding Management Publishing"
	ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
}

Update-MgBetaUserProfilePublication -UserId $userId -ItemPublicationId $itemPublicationId -BodyParameter $params

```