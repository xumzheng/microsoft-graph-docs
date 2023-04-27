---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Sites

$params = @{
	fields = @{
		Title = "Widget"
		Color = "Purple"
		Weight = 32
	}
}

New-MgSiteListItem -SiteId $siteId -ListId $listId -BodyParameter $params

```