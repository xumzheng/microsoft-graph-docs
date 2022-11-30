---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Sites

$params = @{
	Fields = @{
		Title = "Widget"
		Color = "Purple"
		Weight = 
	}
}

New-MgSiteListItem -SiteId $siteId -ListId $listId -BodyParameter $params

```