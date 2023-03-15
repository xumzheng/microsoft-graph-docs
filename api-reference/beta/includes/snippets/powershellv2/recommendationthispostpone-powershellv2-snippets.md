---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	PostponeUntilDateTime = [System.DateTime]::Parse("2023-02-01T02:53:00Z")
}

Invoke-MgBetaPostponeDirectoryRecommendation -RecommendationId $recommendationId -BodyParameter $params

```