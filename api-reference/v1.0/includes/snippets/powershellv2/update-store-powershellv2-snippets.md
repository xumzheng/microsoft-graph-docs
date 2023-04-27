---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Sites

$params = @{
	defaultLanguageTag = "en-US"
}

Update-MgSiteTermStore -SiteId $siteId -BodyParameter $params

```