---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Sites

$params = @{
	Color = "Fuchsia"
	Quantity = 934
}

Update-MgBetaSiteListItemField -SiteId $siteId -ListId $listId -ListItemId $listItemId -BodyParameter $params

```