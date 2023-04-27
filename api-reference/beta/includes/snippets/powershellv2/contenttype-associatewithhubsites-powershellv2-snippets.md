---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Sites

$params = @{
	hubSiteUrls = @(
		"https://graph.microsoft.com/beta/sites/id"
	)
	propagateToExistingLists = $false
}

Join-MgBetaSiteContentTypeWithHubSite -SiteId $siteId -ContentTypeId $contentTypeId -BodyParameter $params

```