---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Sites

$params = @{
	description = "mySet"
}

Update-MgSiteTermStoreSet -SiteId $siteId -SetId $setId -BodyParameter $params

```