---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Sites

$params = @{
	ContentType = "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101"
}

Add-MgBetaSiteListContentTypeCopy -SiteId $siteId -ListId $listId -BodyParameter $params

```