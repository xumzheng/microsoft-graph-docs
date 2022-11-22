---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Sites

$params = @{
	Name = "docSet"
	Description = "custom docset"
	Base = @{
		Name = "Document Set"
		Id = "0x0120D520"
	}
	Group = "Document Set Content Types"
}

New-MgBetaSiteContentType -SiteId $siteId -BodyParameter $params

```