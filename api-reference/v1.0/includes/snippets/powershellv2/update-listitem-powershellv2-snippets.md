---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Sites

$params = @{
	Color = "Fuchsia"
	Quantity = 934
}

Update-MgSiteListItemField -SiteId $siteId -ListId $listId -ListItemId $listItemId -BodyParameter $params

```