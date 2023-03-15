---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	DismissReason = "Recommendations is not relevant for my organization because..."
}

Invoke-MgBetaDismissDirectoryRecommendation -RecommendationId $recommendationId -BodyParameter $params

```