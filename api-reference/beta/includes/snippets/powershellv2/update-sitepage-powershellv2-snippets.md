---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Sites

$params = @{
	"@odata.type" = "#microsoft.graph.sitePage"
	title = "sample"
	showComments = $true
	showRecommendedPages = $false
}

Update-MgBetaSitePage -SiteId $siteId -SitePageId $sitePageId -BodyParameter $params

```