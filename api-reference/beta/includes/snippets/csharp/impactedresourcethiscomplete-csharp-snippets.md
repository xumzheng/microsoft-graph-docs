---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.Recommendations["{recommendation-id}"].ImpactedResources["{impactedResource-id}"]
	.Complete()
	.Request()
	.PostAsync();

```