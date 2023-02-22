---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var impactedResources = await graphClient.Directory.Recommendations["{recommendation-id}"].ImpactedResources
	.Request()
	.GetAsync();

```