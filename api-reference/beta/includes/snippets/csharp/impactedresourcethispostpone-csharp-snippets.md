---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var postponeUntilDateTime = DateTimeOffset.Parse("2023-03-01T09:40:39.0420371Z");

await graphClient.Directory.Recommendations["{recommendation-id}"].ImpactedResources["{impactedResource-id}"]
	.Postpone(postponeUntilDateTime)
	.Request()
	.PostAsync();

```