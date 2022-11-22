---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Sites

$params = @{
	Comment = "v1"
	ShouldCaptureMinorVersion = $false
}

New-MgBetaSiteListItemDocumentSetVersion -SiteId $siteId -ListId $listId -ListItemId $listItemId -BodyParameter $params

```