---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Sites

$params = @{
	Description = "test"
	EnforceUniqueValues = $false
	Hidden = $false
	Indexed = $false
	Name = "Title"
	Text = @{
		AllowMultipleLines = $false
		AppendChangesToExistingText = $false
		LinesForEditing = 0
		MaxLength = 255
	}
}

New-MgBetaSiteColumn -SiteId $siteId -BodyParameter $params

```