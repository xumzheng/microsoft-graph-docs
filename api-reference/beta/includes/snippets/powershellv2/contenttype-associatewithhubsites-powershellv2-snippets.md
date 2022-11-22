---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Sites

$params = @{
	HubSiteUrls = @(
		"https://graph.microsoft.com/beta/sites/id"
	)
	PropagateToExistingLists = $false
}

Join-MgBetaSiteContentTypeWithHubSite -SiteId $siteId -ContentTypeId $contentTypeId -BodyParameter $params

```